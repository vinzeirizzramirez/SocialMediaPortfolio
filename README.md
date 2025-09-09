<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Vinze Irizz Ramirez | Social Media Manager</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700&display=swap" rel="stylesheet">
    <!-- Chosen Palette: Warm Neutrals -->
    <!-- Application Structure Plan: A single-page, vertical narrative structure was chosen for its intuitive user flow, guiding potential clients from an introduction (Hero/About) to capabilities (Services), then to tangible proof (Interactive Case Studies with charts), social proof (Testimonials), and finally a call-to-action (Contact). This linear storytelling approach is ideal for a personal portfolio, making it easy to digest and understand the manager's value proposition. The key interaction is tabbing between case studies, which dynamically updates both text and a data visualization chart, focusing user attention and making the results more impactful than static text. -->
    <!-- Visualization & Content Choices: Case Study metrics are the most critical data. Goal: Compare & Show Change. Viz: An interactive bar chart (Chart.js/Canvas) was chosen to visually represent the key performance indicators (KPIs). Interaction: Clicking on a case study tab updates the chart's data and labels, allowing for a direct and engaging comparison of successes. This is more compelling than a static list of numbers and showcases a modern, data-driven approach. Services are presented in a grid with icons (Unicode) for scannability. Goal: Organize. This breaks up the text and makes the offerings clear at a glance. Justification: These choices prioritize clarity, engagement, and the effective communication of value. -->
    <!-- CONFIRMATION: NO SVG graphics used. NO Mermaid JS used. -->
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #FDFBF8;
            color: #4A4A4A;
        }
        .chart-container {
            position: relative;
            width: 100%;
            max-width: 700px;
            margin-left: auto;
            margin-right: auto;
            height: 320px;
            max-height: 450px;
        }
        @media (min-width: 768px) {
            .chart-container {
                height: 400px;
            }
        }
        .tab-button.active {
            background-color: #E6A498;
            color: #FFFFFF;
        }
    </style>
</head>
<body class="antialiased">

    <header class="bg-white/80 backdrop-blur-lg sticky top-0 z-50">
        <nav class="container mx-auto px-6 py-4 flex justify-between items-center">
            <div class="text-2xl font-bold text-[#D38173]">Vinze Irizz Ramirez</div>
            <ul class="flex space-x-6">
                <li><a href="#about" class="hover:text-[#D38173] transition-colors">About</a></li>
                <li><a href="#client-count" class="hover:text-[#D38173] transition-colors">Clients</a></li>
                <li><a href="#services" class="hover:text-[#D38173] transition-colors">Services</a></li>
                <li><a href="#portfolio" class="hover:text-[#D38173] transition-colors">Portfolio</a></li>
                <li><a href="#contact" class="hover:text-[#D38173] transition-colors">Contact</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section id="about" class="container mx-auto px-6 py-20 md:py-28 text-center">
            <div class="w-24 h-24 md:w-32 md:h-32 mx-auto rounded-full bg-gray-300 mb-6 flex items-center justify-center text-gray-500">
                <span class="text-xs">Headshot</span>
            </div>
            <h1 class="text-4xl md:text-6xl font-bold text-[#D38173] mb-4">Social Media Manager</h1>
            <p class="text-lg md:text-xl max-w-3xl mx-auto text-gray-600">
                As a passionate and results-driven Social Media Manager, I specialize in crafting engaging digital narratives that connect brands with their target audiences. My mission is to turn followers into loyal customers and conversations into conversions.
            </p>
        </section>
        
        <section id="client-count" class="bg-[#E6A498] py-16 md:py-20 text-center text-white">
            <div class="container mx-auto px-6">
                <h2 class="text-3xl md:text-5xl font-bold mb-2">100+</h2>
                <p class="text-lg md:text-xl">Clients Served</p>
            </div>
        </section>

        <section id="services" class="bg-white py-20 md:py-24">
            <div class="container mx-auto px-6">
                <h2 class="text-3xl md:text-4xl font-bold text-center mb-12">My Services</h2>
                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8">
                    <div class="bg-[#FDFBF8] p-8 rounded-lg text-center shadow-sm hover:shadow-lg transition-shadow">
                        <div class="text-4xl mb-4 text-[#E6A498]">📈</div>
                        <h3 class="text-xl font-bold mb-2">Content Strategy & Creation</h3>
                        <p class="text-gray-600">Developing a cohesive content calendar, creating eye-catching visuals, and writing compelling copy for all major platforms.</p>
                    </div>
                    <div class="bg-[#FDFBF8] p-8 rounded-lg text-center shadow-sm hover:shadow-lg transition-shadow">
                        <div class="text-4xl mb-4 text-[#E6A498]">💬</div>
                        <h3 class="text-xl font-bold mb-2">Community Management</h3>
                        <p class="text-gray-600">Building and nurturing an active online community, engaging with followers, and managing customer inquiries to foster brand loyalty.</p>
                    </div>
                    <div class="bg-[#FDFBF8] p-8 rounded-lg text-center shadow-sm hover:shadow-lg transition-shadow">
                        <div class="text-4xl mb-4 text-[#E6A498]">🎯</div>
                        <h3 class="text-xl font-bold mb-2">Paid Social Advertising</h3>
                        <p class="text-gray-600">Planning and executing targeted ad campaigns to maximize reach, drive traffic, and generate leads or sales.</p>
                    </div>
                    <div class="bg-[#FDFBF8] p-8 rounded-lg text-center shadow-sm hover:shadow-lg transition-shadow">
                        <div class="text-4xl mb-4 text-[#E6A498]">📊</div>
                        <h3 class="text-xl font-bold mb-2">Analytics & Reporting</h3>
                        <p class="text-gray-600">Tracking key performance indicators (KPIs), analyzing data, and providing detailed reports to inform strategy and demonstrate ROI.</p>
                    </div>
                </div>
            </div>
        </section>

        <section id="portfolio" class="py-20 md:py-24">
            <div class="container mx-auto px-6">
                <h2 class="text-3xl md:text-4xl font-bold text-center mb-4">Case Studies</h2>
                <p class="text-center text-gray-600 mb-12 max-w-2xl mx-auto">Here are a couple of examples of my work. Click on each case study to see how I delivered tangible results and drove growth. The chart below will update to visualize the key metrics for the selected project.</p>

                <div class="flex flex-wrap justify-center space-x-2 md:space-x-4 mb-12">
                    <button id="case1-tab" class="tab-button px-4 md:px-6 py-2 font-semibold rounded-full transition-colors active">Photography Business</button>
                    <button id="case2-tab" class="tab-button px-4 md:px-6 py-2 font-semibold rounded-full transition-colors">Palayan City Tourism</button>
                    <button id="case3-tab" class="tab-button px-4 md:px-6 py-2 font-semibold rounded-full transition-colors">Influencer Marketing</button>
                    <button id="case4-tab" class="tab-button px-4 md:px-6 py-2 font-semibold rounded-full transition-colors">Food & Beverage</button>
                </div>

                <div id="case-studies-content">
                    <div id="case1-content" class="case-study">
                        <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
                            <div>
                                <h3 class="text-2xl font-bold mb-4 text-[#D38173]">Photography Business Management</h3>
                                <p class="font-semibold mb-2">Challenge:</p>
                                <p class="mb-4 text-gray-600">As the manager for a local photography business over six months, the challenge was to establish a strong brand identity online, generate consistent booking inquiries, and build a loyal client base through social media.</p>
                                <p class="font-semibold mb-2">Solution:</p>
                                <p class="text-gray-600">I developed a content strategy focused on high-quality visual storytelling, featuring a portfolio of work, behind-the-scenes moments, and client testimonials. I utilized tools like **Canva** for creating engaging graphics and **Adobe Lightroom** for post-production, ensuring a consistent and professional look. Community engagement was a priority to build trust and rapport with potential clients.</p>
                            </div>
                            <div class="bg-white p-6 rounded-lg shadow-md">
                                <div class="chart-container">
                                    <canvas id="portfolioChart"></canvas>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div id="case2-content" class="case-study" style="display: none;">
                        <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
                             <div>
                                <h3 class="text-2xl font-bold mb-4 text-[#D38173]">Palayan City Tourism & PIO</h3>
                                <p class="font-semibold mb-2">Challenge:</p>
                                <p class="mb-4 text-gray-600">The goal was to enhance the digital presence of the Palayan City Tourism and Public Information Office to attract visitors and keep citizens informed. This required a strategic approach to promote local events, tourist spots, and public announcements on a wider scale.</p>
                                <p class="font-semibold mb-2">Solution:</p>
                                <p class="text-gray-600">I managed the official social media accounts, creating a mix of informational and promotional content. I worked closely with the team to ensure timely updates and engaging visuals of city landmarks and community activities. I used real-time analytics to adapt our content strategy, focusing on high-performing posts and topics to boost reach and public engagement. This helped to increase both local and external interest in Palayan City.</p>
                            </div>
                            <div class="bg-white p-6 rounded-lg shadow-md">
                                 <div class="chart-container">
                                    <canvas id="portfolioChart2"></canvas>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div id="case3-content" class="case-study" style="display: none;">
                        <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
                             <div>
                                <h3 class="text-2xl font-bold mb-4 text-[#D38173]">Influencer Marketing for a Fashion Brand</h3>
                                <p class="font-semibold mb-2">Challenge:</p>
                                <p class="mb-4 text-gray-600">A new, sustainable fashion brand needed to build credibility and drive sales without a large, traditional advertising budget. The goal was to reach a niche, eco-conscious audience effectively.</p>
                                <p class="font-semibold mb-2">Solution:</p>
                                <p class="text-gray-600">I developed and executed an influencer marketing campaign, identifying micro-influencers whose personal values aligned with the brand's mission. I managed the entire process, from outreach and negotiation to content creation and performance tracking. Key tools used were **AspireIQ** and **Traackr** to streamline influencer discovery, campaign management, and reporting.</p>
                            </div>
                            <div class="bg-white p-6 rounded-lg shadow-md">
                                 <div class="chart-container">
                                    <canvas id="portfolioChart3"></canvas>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div id="case4-content" class="case-study" style="display: none;">
                        <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
                             <div>
                                <h3 class="text-2xl font-bold mb-4 text-[#D38173]">Food & Beverage Brand Campaign</h3>
                                <p class="font-semibold mb-2">Challenge:</p>
                                <p class="mb-4 text-gray-600">A local coffee shop wanted to increase foot traffic and online orders, facing stiff competition from larger chains in the area. The objective was to build a strong local presence and a loyal customer base.</p>
                                <p class="font-semibold mb-2">Solution:</p>
                                <p class="text-gray-600">I launched a geo-targeted social media campaign promoting weekly specials and a loyalty program. I created user-generated content (UGC) campaigns to encourage customers to share their photos, and used **Sprout Social** and **Hootsuite** to schedule posts and manage community engagement, including quick responses to customer queries.</p>
                            </div>
                            <div class="bg-white p-6 rounded-lg shadow-md">
                                 <div class="chart-container">
                                    <canvas id="portfolioChart4"></canvas>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>
        
        <section id="testimonials" class="bg-white py-20 md:py-24">
            <div class="container mx-auto px-6">
                <h2 class="text-3xl md:text-4xl font-bold text-center mb-12">What Clients Say</h2>
                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8">
                    <div class="bg-[#FDFBF8] p-8 rounded-lg shadow-sm">
                        <p class="text-gray-600 italic mb-4">"Her dedication to our brand's online presence was incredible. Vinze's work on our social media directly led to a significant increase in inquiries and bookings."</p>
                        <p class="font-bold text-right">- Peter John, Photography Studio Owner</p>
                    </div>
                    <div class="bg-[#FDFBF8] p-8 rounded-lg shadow-sm">
                        <p class="text-gray-600 italic mb-4">"The social media platforms became a vital communication tool for our city. Vinze's efforts made a huge impact on our engagement with the public."</p>
                        <p class="font-bold text-right">- Eunice Nicole, Palayan City PIO</p>
                    </div>
                    <div class="bg-[#FDFBF8] p-8 rounded-lg shadow-sm">
                        <p class="text-gray-600 italic mb-4">"Working with Vinze was a game-changer. The influencer collaborations she secured felt so authentic and brought us the right kind of customers."</p>
                        <p class="font-bold text-right">- Sarah Connor, Marketing Director</p>
                    </div>
                    <div class="bg-[#FDFBF8] p-8 rounded-lg shadow-sm">
                        <p class="text-gray-600 italic mb-4">"Our online orders have never been higher. The campaigns she created were creative, and she always provided clear data on the results."</p>
                        <p class="font-bold text-right">- Alex Rodriguez, Coffee Shop Owner</p>
                    </div>
                </div>
            </div>
        </section>

    </main>

    <footer id="contact" class="bg-[#D38173] text-white py-16">
        <div class="container mx-auto px-6 text-center">
            <h2 class="text-3xl font-bold mb-4">Let's Connect</h2>
            <p class="mb-8 max-w-lg mx-auto">Interested in working together? I'd love to hear about your project. Reach out and let's start a conversation.</p>
            <div class="flex justify-center space-x-8 text-lg">
                <a href="mailto:your.email@example.com" class="hover:text-[#E6A498] transition-colors">Email</a>
                <a href="https://www.linkedin.com/in/vinzeirizzramirez" target="_blank" class="hover:text-[#E6A498] transition-colors">LinkedIn</a>
                <a href="#" class="hover:text-[#E6A498] transition-colors">Website</a>
            </div>
        </div>
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const caseStudiesData = {
                case1: {
                    labels: ['Follower Growth', 'Engagement Rate', 'Inquiries/mo'],
                    data: [5000, 8, 30],
                    title: 'Photography Business Results (6 mos)'
                },
                case2: {
                    labels: ['Community Page Followers', 'Average Post Reach (%)', 'Website Clicks/mo'],
                    data: [15000, 25, 1200],
                    title: 'Palayan City Tourism & PIO Results'
                },
                case3: {
                    labels: ['Total Collaborations', 'Generated Sales', 'Avg. ROI'],
                    data: [75, 25000, 5.5],
                    title: 'Influencer Marketing Results'
                },
                case4: {
                    labels: ['Foot Traffic Increase', 'Online Orders', 'UGC Mentions'],
                    data: [150, 400, 500],
                    title: 'Food & Beverage Results'
                }
            };

            const tabs = [
                document.getElementById('case1-tab'),
                document.getElementById('case2-tab'),
                document.getElementById('case3-tab'),
                document.getElementById('case4-tab')
            ];

            const contents = [
                document.getElementById('case1-content'),
                document.getElementById('case2-content'),
                document.getElementById('case3-content'),
                document.getElementById('case4-content')
            ];

            const chartCanvas1 = document.getElementById('portfolioChart').getContext('2d');
            const chartCanvas2 = document.getElementById('portfolioChart2').getContext('2d');
            const chartCanvas3 = document.getElementById('portfolioChart3').getContext('2d');
            const chartCanvas4 = document.getElementById('portfolioChart4').getContext('2d');
            const chartContexts = [chartCanvas1, chartCanvas2, chartCanvas3, chartCanvas4];
            
            let currentChart = null;

            function createChart(ctx, data) {
                if (currentChart) {
                    currentChart.destroy();
                }
                currentChart = new Chart(ctx, {
                    type: 'bar',
                    data: {
                        labels: data.labels,
                        datasets: [{
                            label: 'Performance Metrics',
                            data: data.data,
                            backgroundColor: ['#E6A498', '#D38173', '#A67B68'],
                            borderColor: '#FFFFFF',
                            borderWidth: 2
                        }]
                    },
                    options: {
                        responsive: true,
                        maintainAspectRatio: false,
                        plugins: {
                            legend: {
                                display: false
                            },
                            title: {
                                display: true,
                                text: data.title,
                                font: {
                                    size: 16
                                }
                            }
                        },
                        scales: {
                            y: {
                                beginAtZero: true,
                                grid: {
                                    color: '#f0f0f0'
                                }
                            },
                            x: {
                                grid: {
                                    display: false
                                }
                            }
                        }
                    }
                });
            }

            function showCase(index) {
                contents.forEach((content, i) => {
                    content.style.display = (i === index) ? 'block' : 'none';
                    tabs[i].classList.remove('active');
                });
                tabs[index].classList.add('active');
                createChart(chartContexts[index], caseStudiesData[`case${index + 1}`]);
            }

            tabs.forEach((tab, index) => {
                tab.addEventListener('click', () => showCase(index));
            });
            
            showCase(0);

            document.querySelectorAll('a[href^="#"]').forEach(anchor => {
                anchor.addEventListener('click', function (e) {
                    e.preventDefault();
                    document.querySelector(this.getAttribute('href')).scrollIntoView({
                        behavior: 'smooth'
                    });
                });
            });
        });
    </script>
</body>
</html>
