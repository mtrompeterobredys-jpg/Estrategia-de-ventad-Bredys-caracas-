<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Infografía: Estrategia de Ventas 360° - Equipos, Utensilios y Servicio</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;500;700;900&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Roboto', sans-serif;
            background-color: #F8F9FA;
            color: #2B2D42;
        }
        .bg-vibrant-primary { background-color: #4361EE; }
        .text-vibrant-primary { color: #4361EE; }
        .border-vibrant-primary { border-color: #4361EE; }
        .bg-vibrant-secondary { background-color: #F72585; }
        .text-vibrant-secondary { color: #F72585; }
        .bg-vibrant-tertiary { background-color: #4CC9F0; }
        .text-vibrant-tertiary { color: #4CC9F0; }
        .bg-vibrant-quaternary { background-color: #7209B7; }
        .text-vibrant-quaternary { color: #7209B7; }

        .chart-container {
            position: relative;
            width: 100%;
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
            height: 350px;
            max-height: 400px;
        }
        @media (min-width: 768px) {
            .chart-container {
                height: 400px;
            }
        }
        .material-card {
            background-color: #FFFFFF;
            border-radius: 0.75rem;
            box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1), 0 2px 4px -1px rgba(0, 0, 0, 0.06);
            padding: 1.5rem;
            transition: transform 0.2s ease-in-out, box-shadow 0.2s ease-in-out;
        }
        .material-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05);
        }
    </style>
</head>
<body class="antialiased pb-12">

    <!--
        PALETTE NAME: Vibrant Sunset Tech (Material Adapted)
        
        CONFIRMATION: NEITHER Mermaid JS NOR SVG were used anywhere in the output.
        
        NARRATIVE PLAN:
        1. Intro: Define the 360° approach (Hardware, Software/Utensils, Service).
        2. Section 1 (Strategic Entry Points): Specific scenarios for Equipos vs Utensilios.
        3. Section 2 (Product-Service Synergy): Visualize how Service drives Equipment sales and vice versa.
        4. Section 3 (Sales Arguments): Breakdown for each category.
    -->

    <header class="bg-vibrant-primary text-white py-12 px-6 shadow-md mb-10">
        <div class="max-w-6xl mx-auto">
            <h1 class="text-4xl md:text-5xl font-black mb-4 tracking-tight">Estrategia 360°: Equipos, Utensilios y Servicio</h1>
            <p class="text-xl md:text-2xl font-light opacity-90 max-w-3xl">Maximizando el valor del cliente a través de la solución integral de cocina.</p>
        </div>
    </header>

    <main class="max-w-6xl mx-auto px-6 space-y-16">

        <section>
            <div class="mb-8">
                <h2 class="text-3xl font-bold text-gray-800 border-l-4 border-vibrant-secondary pl-4 mb-4">1. El Trípode de Venta</h2>
                <p class="text-lg text-gray-600 italic">No vendes un objeto, vendes la capacidad operativa de una cocina profesional.</p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
                <div class="material-card border-b-4 border-vibrant-primary">
                    <div class="text-4xl mb-4 text-center">🔥</div>
                    <h3 class="text-xl font-bold text-center mb-2">Equipos Pesados</h3>
                    <p class="text-sm text-gray-600 text-center">Hornos, estufas, frío. Es la inversión de capital (CAPEX) del cliente. Venta de alto valor y ciclo largo.</p>
                </div>
                <div class="material-card border-b-4 border-vibrant-secondary">
                    <div class="text-4xl mb-4 text-center">🔪</div>
                    <h3 class="text-xl font-bold text-center mb-2">Utensilios</h3>
                    <p class="text-sm text-gray-600 text-center">Cuchillería, ollas, menaje. Gasto operativo (OPEX). Venta de alta rotación y puerta de entrada rápida.</p>
                </div>
                <div class="material-card border-b-4 border-vibrant-tertiary">
                    <div class="text-4xl mb-4 text-center">🛠️</div>
                    <h3 class="text-xl font-bold text-center mb-2">Servicio Técnico</h3>
                    <p class="text-sm text-gray-600 text-center">Mantenimiento y reparación. El generador de confianza y recurrencia mensual.</p>
                </div>
            </div>
        </section>

        <section class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
            <div>
                <h2 class="text-3xl font-bold text-gray-800 mb-6">Sinergia de Categorías</h2>
                <p class="text-gray-600 mb-6">Visualizamos cómo interactúan tus tres líneas de negocio. El servicio técnico a menudo detecta la necesidad de un equipo nuevo, mientras que los utensilios mantienen el flujo de caja activo.</p>
                <div class="chart-container">
                    <canvas id="radarChart"></canvas>
                </div>
                <p class="text-xs text-gray-400 mt-4 text-center italic">Este gráfico muestra la intensidad de esfuerzo vs. retorno por categoría.</p>
            </div>

            <div class="space-y-4">
                <h3 class="text-xl font-bold text-vibrant-primary">Estrategias de "Cross-Selling"</h3>
                <div class="material-card bg-gray-50 border-none shadow-none">
                    <h4 class="font-bold flex items-center"><span class="mr-2">🔄</span> De Servicio a Equipo</h4>
                    <p class="text-sm text-gray-600 italic">"Este horno ya requiere reparaciones constantes; es el momento de invertir en uno de nueva generación que le ahorrará un 20% de energía."</p>
                </div>
                <div class="material-card bg-gray-50 border-none shadow-none">
                    <h4 class="font-bold flex items-center"><span class="mr-2">🔄</span> De Utensilio a Confianza</h4>
                    <p class="text-sm text-gray-600 italic">"Pruebe estos cuchillos de alto rendimiento. Si le gusta la calidad, hablemos de cómo optimizar su línea de cocción."</p>
                </div>
                <div class="material-card bg-gray-50 border-none shadow-none">
                    <h4 class="font-bold flex items-center"><span class="mr-2">🔄</span> De Equipo a Servicio</h4>
                    <p class="text-sm text-gray-600 italic">"Con su nueva estufa industrial, le incluimos los primeros 6 meses de mantenimiento preventivo gratis."</p>
                </div>
            </div>
        </section>

        <section class="bg-white rounded-2xl shadow-sm border border-gray-100 p-8">
            <h2 class="text-3xl font-bold text-gray-800 text-center mb-10">Potencial de Margen vs Recurrencia</h2>
            <div class="chart-container mb-8">
                <canvas id="bubbleChart"></canvas>
            </div>
            <div class="grid grid-cols-1 md:grid-cols-3 gap-6 text-center">
                <div class="p-4 bg-blue-50 rounded-lg">
                    <p class="font-black text-vibrant-primary text-2xl">Equipos</p>
                    <p class="text-xs uppercase text-gray-500 tracking-widest">Alto Margen / Baja Recurrencia</p>
                </div>
                <div class="p-4 bg-pink-50 rounded-lg">
                    <p class="font-black text-vibrant-secondary text-2xl">Utensilios</p>
                    <p class="text-xs uppercase text-gray-500 tracking-widest">Bajo Margen / Alta Recurrencia</p>
                </div>
                <div class="p-4 bg-cyan-50 rounded-lg">
                    <p class="font-black text-vibrant-tertiary text-2xl">Servicio</p>
                    <p class="text-xs uppercase text-gray-500 tracking-widest">Margen Estable / Alta Fidelidad</p>
                </div>
            </div>
        </section>

    </main>

    <footer class="mt-20 bg-gray-900 text-white py-12 px-6">
        <div class="max-w-4xl mx-auto text-center">
            <h3 class="text-2xl font-bold mb-4">¿Listo para la próxima visita?</h3>
            <p class="text-gray-400 mb-8">Recuerda: Si el cliente no tiene presupuesto para un horno hoy, seguramente necesita renovar sus cuchillos o reparar una fuga de gas.</p>
            <div class="flex flex-wrap justify-center gap-4">
                <span class="px-6 py-2 bg-vibrant-primary rounded-full font-bold">Venta Consultiva</span>
                <span class="px-6 py-2 bg-vibrant-secondary rounded-full font-bold">Post-Venta Activa</span>
                <span class="px-6 py-2 bg-vibrant-tertiary rounded-full font-bold text-gray-900">Solución 360°</span>
            </div>
        </div>
    </footer>

    <script>
        // Data processing for Chart.js labels (16 char rule)
        const wrapLabel = (label) => {
            if (label.length <= 16) return label;
            const words = label.split(' ');
            const lines = [];
            let currentLine = "";
            words.forEach(word => {
                if ((currentLine + word).length > 16) {
                    lines.push(currentLine.trim());
                    currentLine = word + " ";
                } else {
                    currentLine += word + " ";
                }
            });
            lines.push(currentLine.trim());
            return lines;
        };

        const tooltipConfig = {
            callbacks: {
                title: function(tooltipItems) {
                    const item = tooltipItems;
                    let label = item.chart.data.labels[item.dataIndex];
                    return Array.isArray(label) ? label.join(' ') : label;
                }
            }
        };

        window.onload = function() {
            // Radar Chart: Comparing Profile Strengths
            new Chart(document.getElementById('radarChart'), {
                type: 'radar',
                data: {
                    labels: [
                        wrapLabel('Margen de Ganancia'),
                        wrapLabel('Frecuencia de Compra'),
                        wrapLabel('Fidelización Cliente'),
                        wrapLabel('Esfuerzo de Venta'),
                        wrapLabel('Conocimiento Técnico')
                    ],
                    datasets: [
                        {
                            label: 'Equipos',
                            data:,
                            borderColor: '#4361EE',
                            backgroundColor: 'rgba(67, 97, 238, 0.2)',
                            pointBackgroundColor: '#4361EE'
                        },
                        {
                            label: 'Utensilios',
                            data:,
                            borderColor: '#F72585',
                            backgroundColor: 'rgba(247, 37, 133, 0.2)',
                            pointBackgroundColor: '#F72585'
                        },
                        {
                            label: 'Servicio',
                            data:,
                            borderColor: '#4CC9F0',
                            backgroundColor: 'rgba(76, 201, 240, 0.2)',
                            pointBackgroundColor: '#4CC9F0'
                        }
                    ]
                },
                options: {
                    responsive: true,
                    maintainAspectRatio: false,
                    plugins: { tooltip: tooltipConfig },
                    scales: {
                        r: {
                            angleLines: { display: true },
                            suggestedMin: 0,
                            suggestedMax: 100
                        }
                    }
                }
            });

            // Bubble Chart: Mapping Profit vs Recurrence
            new Chart(document.getElementById('bubbleChart'), {
                type: 'bubble',
                data: {
                    datasets: [
                        {
                            label: 'Equipos Pesados',
                            data: [{x: 20, y: 90, r: 40}], // x: Recurrence, y: Margin, r: Value
                            backgroundColor: '#4361EE'
                        },
                        {
                            label: 'Utensilios',
                            data: [{x: 85, y: 35, r: 25}],
                            backgroundColor: '#F72585'
                        },
                        {
                            label: 'Servicio Técnico',
                            data: [{x: 75, y: 65, r: 30}],
                            backgroundColor: '#4CC9F0'
                        }
                    ]
                },
                options: {
                    responsive: true,
                    maintainAspectRatio: false,
                    plugins: {
                        tooltip: tooltipConfig,
                        legend: { position: 'bottom' }
                    },
                    scales: {
                        x: {
                            title: { display: true, text: 'Frecuencia de Compra (Recurrencia)' },
                            min: 0, max: 100
                        },
                        y: {
                            title: { display: true, text: 'Margen de Ganancia (%)' },
                            min: 0, max: 100
                        }
                    }
                }
            });
        };
    </script>
</body>
</html>
