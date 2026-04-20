<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>The Haven | 연예인 전문 심리·영성 케어 센터</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <link href="https://fonts.googleapis.com/css2?family=Noto+Sans+KR:wght@300;400;500;700&family=Nanum+Myeongjo:wght@400;700&display=swap" rel="stylesheet">
    
    <!-- Chosen Palette: Warm Neutrals & Sage -->
    <style>
        body {
            font-family: 'Noto Sans KR', sans-serif;
            background-color: #fbfaf6;
            color: #2c3e2e;
            scroll-behavior: smooth;
            margin: 0;
            padding: 0;
        }
        h1, h2, h3, .serif {
            font-family: 'Nanum Myeongjo', serif;
        }
        
        /* Chart Container Requirements */
        .chart-container {
            position: relative;
            width: 100%;
            max-width: 800px;
            margin-left: auto;
            margin-right: auto;
            height: 40vh;
            max-height: 400px;
        }
        @media (min-width: 768px) {
            .chart-container { height: 50vh; max-height: 450px; }
        }

        /* Tab Animations */
        .tab-content { display: none; opacity: 0; transition: opacity 0.4s ease-in-out; }
        .tab-content.active { display: block; opacity: 1; }
        
        /* Custom UI Elements */
        .glass-panel {
            background: rgba(255, 255, 255, 0.6);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.3);
        }
    </style>
</head>
<body class="antialiased selection:bg-[#6b7c62] selection:text-white">

    <!-- Navigation -->
    <nav class="fixed w-full z-50 glass-panel transition-all duration-300" id="navbar">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between h-20 items-center">
                <div class="flex-shrink-0">
                    <a href="#" class="text-2xl font-bold serif text-[#6b7c62] tracking-widest">THE HAVEN</a>
                </div>
                <div class="hidden md:flex space-x-8">
                    <a href="#about" class="text-sm uppercase tracking-wide hover:text-[#6b7c62] transition-colors">Philosophy</a>
                    <a href="#programs" class="text-sm uppercase tracking-wide hover:text-[#6b7c62] transition-colors">Programs</a>
                    <a href="#space" class="text-sm uppercase tracking-wide hover:text-[#6b7c62] transition-colors">Space & Safety</a>
                    <a href="#impact" class="text-sm uppercase tracking-wide hover:text-[#6b7c62] transition-colors">Impact</a>
                </div>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="relative pt-32 pb-20 lg:pt-48 lg:pb-32 flex items-center justify-center min-h-[80vh]">
        <div class="absolute inset-0 overflow-hidden pointer-events-none">
            <div class="absolute -top-40 -right-40 w-96 h-96 bg-[#d4c5b9] rounded-full mix-blend-multiply filter blur-3xl opacity-30"></div>
            <div class="absolute -bottom-40 -left-40 w-96 h-96 bg-[#6b7c62] rounded-full mix-blend-multiply filter blur-3xl opacity-20"></div>
        </div>
        
        <div class="max-w-4xl mx-auto px-4 text-center relative z-10">
            <p class="text-sm uppercase tracking-[0.3em] text-[#6b7c62] mb-4 font-semibold">연예인 전문 심리·영성 케어 센터</p>
            <h1 class="text-5xl md:text-6xl font-bold mb-6 leading-tight">가면을 벗고,<br>진정한 안식을 누리는 곳</h1>
            <p class="text-lg md:text-xl text-gray-600 mb-10 max-w-2xl mx-auto leading-relaxed">
                대중의 시선과 평판의 압박에서 벗어나세요. 철저한 보안 속에서 성경적 원리와 예술적 도구를 통해 무너진 내면을 치유하고 단단한 자아를 회복합니다.
            </p>
            <a href="#about" class="inline-block px-8 py-3 bg-[#6b7c62] text-white rounded-none hover:bg-[#52604b] transition-colors duration-300 text-sm tracking-widest uppercase">
                Discover The Haven
            </a>
        </div>
    </section>

    <!-- Core Values Section -->
    <section id="about" class="py-20 bg-white">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-3xl font-bold serif mb-4">우리의 철학 (Core Values)</h2>
                <p class="text-gray-600 max-w-2xl mx-auto">더 헤이븐은 VVIP 내담자의 특수성을 완벽히 이해하며, 안전한 환경 속에서 전인적인 회복을 돕기 위해 세 가지 핵심 가치를 지킵니다.</p>
            </div>
            
            <div class="grid md:grid-cols-3 gap-8">
                <div class="p-8 border border-gray-100 hover:shadow-xl transition-shadow duration-300 bg-[#fbfaf6] group text-center rounded-sm">
                    <div class="text-4xl mb-4 group-hover:scale-110 transition-transform duration-300">🤫</div>
                    <h3 class="text-xl font-bold mb-3">Strict Confidentiality</h3>
                    <h4 class="text-sm font-semibold text-[#6b7c62] mb-3">철저한 보안</h4>
                    <p class="text-gray-600 text-sm leading-relaxed">일반 상담소 방문 시 발생할 수 있는 유출 우려를 원천 차단합니다. 전용 출입구와 100% 사전 예약제를 통한 1:1 프라이빗 케어를 제공합니다.</p>
                </div>
                <div class="p-8 border border-gray-100 hover:shadow-xl transition-shadow duration-300 bg-[#fbfaf6] group text-center rounded-sm">
                    <div class="text-4xl mb-4 group-hover:scale-110 transition-transform duration-300">🌱</div>
                    <h3 class="text-xl font-bold mb-3">Holistic Healing</h3>
                    <h4 class="text-sm font-semibold text-[#6b7c62] mb-3">전인적 치유</h4>
                    <p class="text-gray-600 text-sm leading-relaxed">단순한 증상 완화를 넘어, 정신(Mind), 감정(Emotion), 그리고 영성(Spirit)의 통합적 회복을 통해 근본적인 문제 해결에 접근합니다.</p>
                </div>
                <div class="p-8 border border-gray-100 hover:shadow-xl transition-shadow duration-300 bg-[#fbfaf6] group text-center rounded-sm">
                    <div class="text-4xl mb-4 group-hover:scale-110 transition-transform duration-300">🎨</div>
                    <h3 class="text-xl font-bold mb-3">Creative Expression</h3>
                    <h4 class="text-sm font-semibold text-[#6b7c62] mb-3">창조적 발산</h4>
                    <p class="text-gray-600 text-sm leading-relaxed">언어만으로는 표현하기 힘든 억눌린 고통과 감정을 음악과 미술이라는 예술적 도구(Catharsis)를 통해 건강한 에너지로 전환합니다.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Programs Section -->
    <section id="programs" class="py-24 bg-[#fbfaf6]">
        <div class="max-w-5xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-12">
                <h2 class="text-3xl font-bold serif mb-4">주요 프로그램</h2>
                <p class="text-gray-600">더 헤이븐의 치료는 성경적 영성을 바탕으로 내면의 정체성을 세우고, 예술 치료를 통해 감정을 해소하는 유기적인 과정으로 구성됩니다.</p>
            </div>

            <div class="flex flex-wrap border-b border-gray-300 mb-8 justify-center">
                <button class="tab-link px-6 py-4 text-sm uppercase tracking-wide font-bold text-[#6b7c62] border-b-2 border-[#6b7c62] focus:outline-none transition-colors" onclick="openProgram(event, 'prog-bible')">
                    영성 상담
                </button>
                <button class="tab-link px-6 py-4 text-sm uppercase tracking-wide text-gray-500 border-b-2 border-transparent hover:text-gray-700 focus:outline-none transition-colors" onclick="openProgram(event, 'prog-music')">
                    음악 치료
                </button>
                <button class="tab-link px-6 py-4 text-sm uppercase tracking-wide text-gray-500 border-b-2 border-transparent hover:text-gray-700 focus:outline-none transition-colors" onclick="openProgram(event, 'prog-art')">
                    미술 치료
                </button>
            </div>

            <div class="bg-white p-8 md:p-12 shadow-sm border border-gray-100 min-h-[300px]">
                <div id="prog-bible" class="tab-content active">
                    <div class="flex flex-col md:flex-row gap-8 items-start">
                        <div class="md:w-1/3">
                            <div class="text-5xl mb-4">📖</div>
                            <h3 class="text-2xl font-bold serif text-[#6b7c62] mb-2">Rooted in Word</h3>
                            <p class="text-sm font-semibold uppercase tracking-widest text-gray-400 mb-4">성경 기반 영성 상담</p>
                        </div>
                        <div class="md:w-2/3">
                            <p class="text-gray-700 mb-6 leading-relaxed">센터의 가장 핵심적인 프로그램입니다. 화려한 연예계 생활 속에서 흔들리기 쉬운 자아를 성경적 원리에 기반하여 단단하게 재건합니다.</p>
                            <ul class="space-y-4">
                                <li class="flex items-start">
                                    <span class="text-[#d4c5b9] mr-3 font-bold">■</span>
                                    <div>
                                        <h4 class="font-bold text-gray-900">정체성 회복 상담</h4>
                                        <p class="text-sm text-gray-600 mt-1">'인기'나 '대중의 평가'가 아닌, 절대자 앞에서의 고유한 존재 가치를 확인하고 자존감을 회복합니다.</p>
                                    </div>
                                </li>
                                <li class="flex items-start">
                                    <span class="text-[#d4c5b9] mr-3 font-bold">■</span>
                                    <div>
                                        <h4 class="font-bold text-gray-900">광야(Wilderness) 세미나</h4>
                                        <p class="text-sm text-gray-600 mt-1">공백기나 슬럼프, 실패의 경험을 좌절이 아닌 영적 도약과 내면 성장의 시기로 재해석하도록 돕습니다.</p>
                                    </div>
                                </li>
                                <li class="flex items-start">
                                    <span class="text-[#d4c5b9] mr-3 font-bold">■</span>
                                    <div>
                                        <h4 class="font-bold text-gray-900">말씀 묵상 및 기도</h4>
                                        <p class="text-sm text-gray-600 mt-1">모든 사회적 가면을 벗고, 안전한 공간에서 온전한 영적 안식과 평안을 누리는 시간을 가집니다.</p>
                                    </div>
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>

                <div id="prog-music" class="tab-content">
                    <div class="flex flex-col md:flex-row gap-8 items-start">
                        <div class="md:w-1/3">
                            <div class="text-5xl mb-4">🎵</div>
                            <h3 class="text-2xl font-bold serif text-[#6b7c62] mb-2">Harmony of Soul</h3>
                            <p class="text-sm font-semibold uppercase tracking-widest text-gray-400 mb-4">전문 음악 치료</p>
                        </div>
                        <div class="md:w-2/3">
                            <p class="text-gray-700 mb-6 leading-relaxed">연예인들에게 친숙한 '음악'이라는 매개를 통해, 방어기제를 허물고 내면 깊은 곳의 상처와 억압된 감정을 안전하게 표출합니다.</p>
                            <ul class="space-y-4">
                                <li class="flex items-start">
                                    <span class="text-[#d4c5b9] mr-3 font-bold">■</span>
                                    <div>
                                        <h4 class="font-bold text-gray-900">송라이팅(Songwriting) 테라피</h4>
                                        <p class="text-sm text-gray-600 mt-1">논리적 언어로 표현하기 힘든 고통과 감정을 가사와 선율로 만들어 내면의 진실된 목소리를 밖으로 꺼냅니다.</p>
                                    </div>
                                </li>
                                <li class="flex items-start">
                                    <span class="text-[#d4c5b9] mr-3 font-bold">■</span>
                                    <div>
                                        <h4 class="font-bold text-gray-900">보컬 브리딩(Vocal Breathing)</h4>
                                        <p class="text-sm text-gray-600 mt-1">올바른 호흡과 발성 훈련을 통해 신체적 긴장을 완화하고, 무대 공포증이나 공황 증상 완화를 적극적으로 지원합니다.</p>
                                    </div>
                                </li>
                                <li class="flex items-start">
                                    <span class="text-[#d4c5b9] mr-3 font-bold">■</span>
                                    <div>
                                        <h4 class="font-bold text-gray-900">악기 즉흥 연주</h4>
                                        <p class="text-sm text-gray-600 mt-1">정해진 형식이나 평가에 대한 부담 없이 악기를 두드리고 연주하며 감정의 응어리를 해소합니다.</p>
                                    </div>
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>

                <div id="prog-art" class="tab-content">
                    <div class="flex flex-col md:flex-row gap-8 items-start">
                        <div class="md:w-1/3">
                            <div class="text-5xl mb-4">🖼️</div>
                            <h3 class="text-2xl font-bold serif text-[#6b7c62] mb-2">Canvas of Grace</h3>
                            <p class="text-sm font-semibold uppercase tracking-widest text-gray-400 mb-4">전문 미술 치료</p>
                        </div>
                        <div class="md:w-2/3">
                            <p class="text-gray-700 mb-6 leading-relaxed">시각적 매체를 활용하여 무의식에 자리 잡은 불안과 혼란을 형태화하고, 객관적으로 바라보며 다듬어가는 과정을 경험합니다.</p>
                            <ul class="space-y-4">
                                <li class="flex items-start">
                                    <span class="text-[#d4c5b9] mr-3 font-bold">■</span>
                                    <div>
                                        <h4 class="font-bold text-gray-900">매체 중심 치료</h4>
                                        <p class="text-sm text-gray-600 mt-1">다양한 매체를 통해 억눌린 무의식을 안전하게 시각화합니다.</p>
                                    </div>
                                </li>
                                <li class="flex items-start">
                                    <span class="text-[#d4c5b9] mr-3 font-bold">■</span>
                                    <div>
                                        <h4 class="font-bold text-gray-900">Self-Portrait 작업</h4>
                                        <p class="text-sm text-gray-600 mt-1">'대중이 보는 나'와 '실제의 나' 사이의 간극을 좁히는 자화상을 작업합니다.</p>
                                    </div>
                                </li>
                                <li class="flex items-start">
                                    <span class="text-[#d4c5b9] mr-3 font-bold">■</span>
                                    <div>
                                        <h4 class="font-bold text-gray-900">Safe Place 만들기</h4>
                                        <p class="text-sm text-gray-600 mt-1">심리적 안정을 주는 가상의 '안전지대'를 구축하여 불안감을 통제하는 힘을 기릅니다.</p>
                                    </div>
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Operations Section -->
    <section id="space" class="py-20 bg-white">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="mb-16">
                <h2 class="text-3xl font-bold serif mb-4">센터 운영 특화 전략</h2>
                <p class="text-gray-600 max-w-2xl">하드웨어와 소프트웨어 양면에서 완벽한 프라이버시를 보장합니다.</p>
            </div>
            <div class="grid md:grid-cols-2 gap-12">
                <div class="bg-[#fbfaf6] p-8 rounded-sm">
                    <h3 class="text-xl font-bold mb-6 border-b border-gray-200 pb-4">🏛️ 공간 기획 (Space)</h3>
                    <ul class="space-y-4 text-sm text-gray-600">
                        <li><strong>VVIP 전용 독립 동선:</strong> 외부 노출 없이 상담실로 직행하는 전용 시스템.</li>
                        <li><strong>최고급 방음 시설:</strong> 감정 표출 과정이 외부로 유출되지 않는 스튜디오급 방음.</li>
                        <li><strong>치유의 실내 정원:</strong> 외부 노출 없이도 자연을 느낄 수 있는 프라이빗 가든.</li>
                    </ul>
                </div>
                <div class="bg-[#fbfaf6] p-8 rounded-sm">
                    <h3 class="text-xl font-bold mb-6 border-b border-gray-200 pb-4">🤝 전문가 네트워킹 (Network)</h3>
                    <ul class="space-y-4 text-sm text-gray-600">
                        <li><strong>다학제적 케어 팀:</strong> 목회 상담, 임상 심리, 예술 치료 전문가가 한 팀으로 케어.</li>
                        <li><strong>긴급 위기 대응 팀:</strong> 갑작스러운 스트레스 사건 발생 시 24시간 긴급 지원.</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- Expected Effects -->
    <section id="impact" class="py-24 bg-[#2c3e2e] text-white">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-12">
                <h2 class="text-3xl font-bold serif mb-4 text-[#fbfaf6]">기대 효과 및 회복 여정</h2>
            </div>
            <div class="grid lg:grid-cols-3 gap-8 items-center">
                <div class="lg:col-span-1 space-y-8 text-sm">
                    <div>
                        <h4 class="text-xl font-bold text-[#d4c5b9] mb-2">1. 영적 기초 확립</h4>
                        <p class="text-gray-400">변하지 않는 절대적 가치관을 통해 삶의 목적을 분명히 확립합니다.</p>
                    </div>
                    <div>
                        <h4 class="text-xl font-bold text-[#d4c5b9] mb-2">2. 건강한 복귀 지원</h4>
                        <p class="text-gray-400">번아웃을 극복하고 강력한 정서적 회복 탄력성을 획득합니다.</p>
                    </div>
                    <div>
                        <h4 class="text-xl font-bold text-[#d4c5b9] mb-2">3. 선한 영향력 전파</h4>
                        <p class="text-gray-400">건강해진 아티스트로서 대중에게 긍정적인 메시지를 전달합니다.</p>
                    </div>
                </div>
                <div class="lg:col-span-2 bg-[#fbfaf6] p-4 md:p-6 rounded-sm shadow-xl">
                    <div class="chart-container">
                        <canvas id="recoveryChart"></canvas>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 text-gray-400 py-12 text-center text-sm">
        <div class="max-w-4xl mx-auto px-4">
            <h2 class="text-2xl font-bold serif text-[#6b7c62] tracking-widest mb-4">THE HAVEN</h2>
            <p>&copy; 2026 The Haven. All rights reserved.</p>
        </div>
    </footer>

    <script>
        window.addEventListener('scroll', () => {
            const nav = document.getElementById('navbar');
            if (window.scrollY > 50) {
                nav.classList.add('shadow-md', 'bg-white/90');
                nav.classList.remove('glass-panel');
            } else {
                nav.classList.remove('shadow-md', 'bg-white/90');
                nav.classList.add('glass-panel');
            }
        });

        function openProgram(evt, programName) {
            const tabcontent = document.getElementsByClassName("tab-content");
            for (let i = 0; i < tabcontent.length; i++) tabcontent[i].classList.remove("active");
            const tablinks = document.getElementsByClassName("tab-link");
            for (let i = 0; i < tablinks.length; i++) {
                tablinks[i].classList.remove("border-[#6b7c62]", "text-[#6b7c62]", "font-bold");
                tablinks[i].classList.add("text-gray-500", "border-transparent");
            }
            document.getElementById(programName).classList.add("active");
            evt.currentTarget.classList.remove("text-gray-500", "border-transparent");
            evt.currentTarget.classList.add("border-[#6b7c62]", "text-[#6b7c62]", "font-bold");
        }

        document.addEventListener('DOMContentLoaded', function() {
            const ctx = document.getElementById('recoveryChart').getContext('2d');
            new Chart(ctx, {
                type: 'line',
                data: {
                    labels: ['입소 전', '프로그램 초기', '중반부', '후반부', '복귀'],
                    datasets: [
                        { label: '번아웃 지수', data: [85, 75, 50, 35, 15], borderColor: '#a39171', fill: false, tension: 0.4 },
                        { label: '회복 탄력성', data: [20, 35, 60, 80, 95], borderColor: '#6b7c62', fill: false, tension: 0.4 }
                    ]
                },
                options: { responsive: true, maintainAspectRatio: false }
            });
        });
    </script>
</body>
</html>
