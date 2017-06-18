
 $(function () {


                var data = [
					{ 'hasc': 'TN.MN', 'name_ar':'أريانة', 'name_ville': 'Ariana', value: 1 , code_js: TN_AN}, //ariana
                    { 'hasc': 'TN.SF', 'name_ar':'صفاقس', 'name_ville': 'Sfax', value: 1 , code_js: TN_SF}, //sfax
                    { 'hasc': 'TN.ME', 'name_ar':'مدنين', 'name_ville': 'Medenine', value: 1 , code_js: TN_ME}, //medenine
                    { 'hasc': 'TN.TO', 'name_ar':'توزر', 'name_ville': 'Tozeur', value: 1 , code_js: TN_TO}, //tozeur
                    { 'hasc': 'TN.AR', 'name_ar':'منوبة', 'name_ville': 'La Manouba', value: 1 , code_js: TN_MN}, //manouba
                    { 'hasc': 'TN.BJ', 'name_ar':'باجة', 'name_ville': 'Beja', value: 1 , code_js: TN_BJ}, //beja
                    { 'hasc': 'TN.BA', 'name_ar':'بن عروس', 'name_ville': 'Ben Arous', value: 1 , code_js: TN_BA}, //ben arous
                    { 'hasc': 'TN.BZ', 'name_ar':'بنزرت', 'name_ville': 'Bizerte', value: 1 , code_js: TN_BZ}, //bizerte
                    { 'hasc': 'TN.JE', 'name_ar':'جندوبة', 'name_ville': 'Jendouba', value: 1 , code_js: TN_JE}, //jendouba
                    { 'hasc': 'TN.NB', 'name_ar':'نابل', 'name_ville': 'Nabeul', value: 1 , code_js: TN_NB}, //nabeul
                    { 'hasc': 'TN.TU', 'name_ar':'تونس', 'name_ville': 'Tunis', value: 1 , code_js: TN_TU}, //tunis
                    { 'hasc': 'TN.KF', 'name_ar':'الكاف', 'name_ville': 'Le Kef', value: 1 , code_js: TN_KF}, //kef
                    { 'hasc': 'TN.KS', 'name_ar':'القصرين', 'name_ville': 'Kasserine', value: 1 , code_js: TN_KS}, //kasserine
                    { 'hasc': 'TN.GB', 'name_ar':'قابس', 'name_ville': 'Gabes', value: 1 , code_js: TN_GB}, //gabes
                    { 'hasc': 'TN.GF', 'name_ar':'قفصة', 'name_ville': 'Gafsa', value: 1 , code_js: TN_GF}, //gafsa
                    { 'hasc': 'TN.SZ', 'name_ar':'سيدي بوزيد', 'name_ville': 'Sidi Bouzid', value: 1 , code_js: TN_SZ}, //sidi bouzid
                    { 'hasc': 'TN.SL', 'name_ar':'سليانـــة', 'name_ville': 'Siliana', value: 1 , code_js: TN_SL}, //siliana
                    { 'hasc': 'TN.MH', 'name_ar':'المهدية', 'name_ville': 'Mahdia', value: 1 , code_js: TN_MH}, //mahdia
                    { 'hasc': 'TN.MS', 'name_ar':'المنستير', 'name_ville': 'Monastir', value: 1 , code_js: TN_MS}, //monastir
                    { 'hasc': 'TN.KR', 'name_ar':'القيروان', 'name_ville': 'Kairouan', value: 1 , code_js: TN_KR}, //kairouan
                    { 'hasc': 'TN.SS', 'name_ar':'سوسة', 'name_ville': 'Sousse', value: 1 , code_js: TN_SS}, //sousse
                    { 'hasc': 'TN.ZA', 'name_ar':'زغوان', 'name_ville': 'Zaghouan', value: 1 , code_js: TN_ZA}, //zaghouan
                    { 'hasc': 'TN.KB', 'name_ar':'قبلي', 'name_ville': 'Kebili', value: 1 , code_js: TN_KB}, // kebili
                    { 'hasc': 'TN.TA', 'name_ar':'تطاوين', 'name_ville': 'Tataouine', value: 1 , code_js: TN_TA}]; //tataouine

            	
                // Initiate the chart
                mapChart = $('#container-map-reforme').highcharts('Map', {
                    
                    title : {
                        text : ''
                    },

                    subtitle : {
                        text : ''
                    },

                    mapNavigation: {
                        enabled: false,
                        buttonOptions: {
                            verticalAlign: 'bottom'
                        }
                    },
					legend: {
						enabled : false,
					},
					colorAxis: {
                    dataClasses: [{
                        to: 1,
					color:'rgba(255,255,255,0)',
                    }],
					}
                ,
					
					plotOptions: {
						series: {
							cursor: 'pointer',
							point: {
								events: {
									click: function () {
									statGov(this.code_js);
									statGovm(this.code_js);
									}
								}
							}
						}
					},
					
                    series : [{
						animation: {
							duration: 1500
						},
                        data : data,
						borderColor:'#ffffff',
						backgroundColor: null,
						borderWidth: 1,
                        mapData: Highcharts.maps['countries/tn/tn-all'],
                        joinBy: 'hasc',
						allowPointSelect: true,
						cursor: 'pointer',
						
                        states: {
				select: {
                			color: '#FFF'
            			},
                            hover: {
							color:'#EEEEEE',
                            }
                        },
						tooltip: {
							headerFormat:'',
							pointFormat: '<span class="f32"><span class="flag {point.name_ville}"></span></span>'
							+ '<span> {point.name_ville} </span><p> '+'<div style="width:15px;"></div>'+'</p>',
						},
                        dataLabels: {
                            enabled: false,
                            format: '{point.name_ville}'
                        }
                    }]
                }).highcharts();


            });
