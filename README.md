<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Infografía: El Ecosistema del Diseñador Gráfico</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;700;900&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
        }
        .chart-container {
            position: relative;
            width: 100%;
            margin-left: auto;
            margin-right: auto;
        }
        .flowchart-step {
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
        }
        .flowchart-arrow {
            font-size: 2rem;
            line-height: 1;
            color: #EB6841;
        }
    </style>
</head>
<body class="bg-gray-100 text-gray-800">

    <div class="container mx-auto p-4 md:p-8">
        
        <header class="text-center mb-12">
            <h1 class="text-4xl md:text-6xl font-black text-[#00A0B0] mb-2">El Ecosistema del Diseñador Gráfico</h1>
            <p class="text-lg md:text-xl text-gray-600 max-w-3xl mx-auto">Un análisis visual de las experiencias laborales que definen la profesión, desde el caos creativo hasta la estrategia corporativa.</p>
        </header>

        <main class="space-y-12">

            <section id="overview" class="bg-white rounded-2xl shadow-lg p-6 md:p-8">
                <h2 class="text-3xl font-bold text-center mb-2 text-[#6A4A3C]">La Realidad del Mercado en Cifras</h2>
                <p class="text-center text-gray-600 mb-8 max-w-2xl mx-auto">La experiencia de un diseñador se divide principalmente en tres arquetipos de proyectos. Esta distribución refleja dónde invierten su tiempo y enfrentan sus mayores desafíos y oportunidades.</p>
                <div class="chart-container max-w-md h-80 md:h-96">
                    <canvas id="workDistributionChart"></canvas>
                </div>
            </section>

            <div class="grid grid-cols-1 lg:grid-cols-2 gap-8">
                
                <section id="category1" class="bg-white rounded-2xl shadow-lg p-6 md:p-8 col-span-1 lg:col-span-2">
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-8 items-center">
                        <div>
                            <h3 class="text-3xl font-bold text-[#CC333F] mb-4">1. Diseño por Gusto Personal</h3>
                            <p class="mb-6 text-gray-600">Representando el <strong class="font-bold text-4xl text-[#CC333F]">45%</strong> de las experiencias, este es el campo de batalla más común. Clientes con poca visión estratégica toman decisiones subjetivas, convirtiendo al diseñador en un ejecutor. Aunque frustrante, es un crisol para forjar habilidades de negociación y comunicación.</p>
                            <div class="space-y-4">
                                <div class="bg-red-50 p-4 rounded-lg border-l-4 border-red-400">
                                    <h4 class="font-bold text-red-800">Desafíos Comunes</h4>
                                    <p class="text-red-700">Briefings ambiguos, cambios interminables y una constante necesidad de justificar el valor profesional.</p>
                                </div>
                                <div class="bg-green-50 p-4 rounded-lg border-l-4 border-green-500">
                                    <h4 class="font-bold text-green-800">Estrategias de Supervivencia</h4>
                                    <p class="text-green-700">Contratos detallados, educar al cliente sobre el proceso y separar el ego del trabajo para enfocarse en la solución.</p>
                                </div>
                            </div>
                        </div>
                        <div class="chart-container max-w-lg h-80 md:h-96">
                            <canvas id="category1Chart"></canvas>
                        </div>
                    </div>
                </section>

                <section id="category2" class="bg-white rounded-2xl shadow-lg p-6 md:p-8">
                    <h3 class="text-3xl font-bold text-[#00A0B0] mb-4">2. Diseño para Marcas Corporativas</h3>
                    <p class="mb-6 text-gray-600">Con un <strong class="font-bold text-4xl text-[#00A0B0]">40%</strong>, este entorno estructurado se rige por manuales de marca y objetivos de negocio. Ofrece estabilidad y crecimiento, pero a menudo limita la libertad creativa a cambio de coherencia y estrategia.</p>
                    <div class="chart-container max-w-lg h-80 md:h-96">
                        <canvas id="category2Chart"></canvas>
                    </div>
                </section>

                <section id="category3" class="bg-white rounded-2xl shadow-lg p-6 md:p-8">
                    <h3 class="text-3xl font-bold text-[#EB6841] mb-4">3. Diseño para Otros Diseñadores</h3>
                    <p class="mb-6 text-gray-600">El <strong class="font-bold text-4xl text-[#EB6841]">15%</strong> restante corresponde a la colaboración entre pares. Es el modelo más eficiente y profesional, pero a menudo implica trabajar como "marca blanca", perdiendo la autoría del proyecto.</p>
                    <div class="h-80 md:h-96 flex flex-col justify-center items-center space-y-2 md:space-y-0 md:space-x-4 md:flex-row">
                        <div class="flowchart-step bg-orange-100 text-orange-800 p-4 rounded-full w-32 h-32 shadow">Diseñador con sobrecarga</div>
                        <div class="flowchart-arrow transform md:-rotate-0 rotate-90">➔</div>
                        <div class="flowchart-step bg-orange-100 text-orange-800 p-4 rounded-full w-32 h-32 shadow">Subcontrata a especialista</div>
                        <div class="flowchart-arrow transform md:-rotate-0 rotate-90">➔</div>
                        <div class="flowchart-step bg-orange-100 text-orange-800 p-4 rounded-full w-32 h-32 shadow">Entrega final (Marca Blanca 👻)</div>
                    </div>
                </section>
            </div>
            
            <section id="conclusion" class="text-center bg-white rounded-2xl shadow-lg p-6 md:p-8">
                <h2 class="text-3xl font-bold text-center mb-4 text-[#6A4A3C]">Conclusión: El Diseñador como Estratega</h2>
                <p class="text-lg text-gray-600 max-w-3xl mx-auto mb-8">El éxito en el diseño gráfico moderno trasciende la habilidad técnica. Requiere una mentalidad de consultor, donde la comunicación, la negociación y la capacidad de demostrar el valor estratégico del diseño son las herramientas más poderosas.</p>
                <div class="flex flex-wrap justify-center items-center gap-4">
                    <span class="bg-[#00A0B0] text-white font-bold text-4xl py-2 px-4 rounded-lg">Estrategia</span>
                    <span class="bg-[#EB6841] text-white font-bold text-2xl py-2 px-4 rounded-lg">Comunicación</span>
                    <span class="bg-[#EDC951] text-[#6A4A3C] font-bold text-xl py-2 px-4 rounded-lg">Negociación</span>
                    <span class="bg-gray-200 text-gray-700 font-bold text-lg py-1 px-3 rounded-lg">Resiliencia</span>
                     <span class="bg-[#CC333F] text-white font-bold text-3xl py-2 px-4 rounded-lg">Valor</span>
                    <span class="bg-gray-200 text-gray-700 font-bold text-md py-1 px-3 rounded-lg">Adaptabilidad</span>
                </div>
            </section>

        </main>
        
        <footer class="text-center mt-12 text-gray-500">
            <p>Infografía generada a partir del análisis de experiencias de diseñadores gráficos.</p>
        </footer>

    </div>

    <script>
        const tooltipTitleCallback = {
            plugins: {
                tooltip: {
                    callbacks: {
                        title: function(tooltipItems) {
                            const item = tooltipItems[0];
                            let label = item.chart.data.labels[item.dataIndex];
                            if (Array.isArray(label)) {
                                return label.join(' ');
                            }
                            return label;
                        }
                    }
                }
            }
        };

        const wrapLabel = (label) => {
            const maxLength = 16;
            if (label.length <= maxLength) return label;
            
            const words = label.split(' ');
            const lines = [];
            let currentLine = '';

            words.forEach(word => {
                if ((currentLine + word).length > maxLength) {
                    lines.push(currentLine.trim());
                    currentLine = '';
                }
                currentLine += word + ' ';
            });
            lines.push(currentLine.trim());
            return lines;
        };

        const workDistributionCtx = document.getElementById('workDistributionChart').getContext('2d');
        new Chart(workDistributionCtx, {
            type: 'doughnut',
            data: {
                labels: ['Diseño por Gusto Personal', 'Diseño para Marcas Corporativas', 'Diseño para Otros Diseñadores'],
                datasets: [{
                    label: 'Distribución de Experiencias',
                    data: [45, 40, 15],
                    backgroundColor: ['#CC333F', '#00A0B0', '#EB6841'],
                    borderColor: '#FFFFFF',
                    borderWidth: 4,
                    hoverOffset: 10
                }]
            },
            options: {
                responsive: true,
                maintainAspectRatio: false,
                plugins: {
                    legend: {
                        position: 'bottom',
                        labels: {
                            padding: 20,
                            font: {
                                size: 14
                            }
                        }
                    },
                    tooltip: tooltipTitleCallback.plugins.tooltip
                },
                cutout: '60%'
            }
        });

        const category1Ctx = document.getElementById('category1Chart').getContext('2d');
        new Chart(category1Ctx, {
            type: 'bar',
            data: {
                labels: ['Falta de Briefing', 'Subjetividad', 'Baja Valoración', 'Comunicación', 'Contratos', 'Educación al Cliente'],
                datasets: [{
                    label: 'Impacto',
                    data: [-8, -9, -7, 7, 9, 8],
                    backgroundColor: (context) => {
                        const value = context.raw;
                        return value < 0 ? 'rgba(204, 51, 63, 0.7)' : 'rgba(0, 160, 176, 0.7)';
                    },
                    borderColor: (context) => {
                        const value = context.raw;
                        return value < 0 ? '#CC333F' : '#00A0B0';
                    },
                    borderWidth: 2
                }]
            },
            options: {
                responsive: true,
                maintainAspectRatio: false,
                indexAxis: 'y',
                scales: {
                    x: {
                        display: false
                    },
                    y: {
                        ticks: {
                            font: {
                                size: 14
                            }
                        }
                    }
                },
                plugins: {
                    legend: {
                        display: false
                    },
                    title: {
                        display: true,
                        text: 'Desafíos (Rojo) vs. Estrategias (Azul)',
                        font: { size: 16 }
                    },
                    tooltip: tooltipTitleCallback.plugins.tooltip
                }
            }
        });

        const category2Ctx = document.getElementById('category2Chart').getContext('2d');
        new Chart(category2Ctx, {
            type: 'radar',
            data: {
                labels: ['Estabilidad', 'Crecimiento', 'Valoración', 'Creatividad', 'Flexibilidad'],
                datasets: [{
                    label: 'Entorno Corporativo',
                    data: [9, 8, 8, 5, 4],
                    fill: true,
                    backgroundColor: 'rgba(0, 160, 176, 0.2)',
                    borderColor: '#00A0B0',
                    pointBackgroundColor: '#00A0B0',
                    pointBorderColor: '#fff',
                    pointHoverBackgroundColor: '#fff',
                    pointHoverBorderColor: '#00A0B0'
                }]
            },
            options: {
                responsive: true,
                maintainAspectRatio: false,
                scales: {
                    r: {
                        angleLines: {
                            display: false
                        },
                        suggestedMin: 0,
                        suggestedMax: 10,
                         pointLabels: {
                            font: {
                                size: 14
                            }
                        }
                    }
                },
                 plugins: {
                    legend: {
                        display: false
                    },
                    tooltip: tooltipTitleCallback.plugins.tooltip
                }
            }
        });
    </script>
</body>
</html>
