<!DOCTYPE html>
<html lang="th">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MOVEFORWARDPATY | OFFICIAL SITE</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Sarabun:wght@100;400;700;800;900&display=swap" rel="stylesheet">
    <script src="https://unpkg.com/scrollreveal"></script>
    <script src="https://unpkg.com/lucide@latest"></script>
    <style>
        :root {
            --blood-maroon: #600000;
            --bright-red: #ff0000;
        }

        body {
            font-family: 'Sarabun', sans-serif;
            background-color: #000;
            color: #fff;
            overflow-x: hidden;
        }

        .hero-title {
            font-size: clamp(3rem, 15vw, 9rem);
            font-weight: 900;
            line-height: 0.8;
            font-style: italic;
            letter-spacing: -0.05em;
        }

        /* ลูกเล่น Paty เรืองแสง d ปกติ */
        .paty-glow {
            color: var(--bright-red);
            text-shadow: 0 0 20px var(--bright-red), 0 0 40px var(--blood-maroon);
            animation: pulse-glow 2s infinite ease-in-out;
        }

        @keyframes pulse-glow {
            0%, 100% { opacity: 1; filter: brightness(1.2); }
            50% { opacity: 0.8; filter: brightness(0.8); }
        }

        .policy-card {
            background: #111;
            border: 1px solid #333;
            transition: all 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            position: relative;
            overflow: hidden;
        }

        .policy-card:hover {
            border-color: var(--bright-red);
            transform: scale(1.02);
            background: #1a0000;
        }

        .policy-card::before {
            content: '';
            position: absolute;
            top: 0; left: 0;
            width: 4px; height: 100%;
            background: var(--bright-red);
        }

        .img-mask {
            mask-image: linear-gradient(to bottom, black 80%, transparent 100%);
            -webkit-mask-image: linear-gradient(to bottom, black 80%, transparent 100%);
        }

        /* แถบสีเลือดหมูวิ่ง */
        .maroon-gradient {
            background: linear-gradient(90deg, #000, var(--blood-maroon), #000);
            background-size: 200% 100%;
            animation: move-bg 5s infinite linear;
        }

        @keyframes move-bg {
            0% { background-position: 200% 0; }
            100% { background-position: -200% 0; }
        }
    </style>
</head>
<body>

    <!-- Nav -->
    <nav class="fixed top-0 w-full z-50 px-10 py-6 flex justify-between items-center bg-black/60 backdrop-blur-lg border-b border-white/5">
        <div class="text-2xl font-black italic tracking-tighter">
            MOVEFORWARD<span class="text-red-600">PATY</span>
        </div>
        <div class="h-2 w-2 bg-red-600 rounded-full animate-ping"></div>
    </nav>

    <!-- Hero -->
    <section class="h-[110vh] flex flex-col items-center justify-center text-center px-6 relative">
        <div class="absolute inset-0 bg-radial-gradient from-red-900/20 to-transparent opacity-50"></div>
        <div class="reveal">
            <h1 class="hero-title">
                MOVE<br>
                FORWAR<span class="text-white">D</span><br>
                <span class="paty-glow uppercase">PATY</span>
            </h1>
            <div class="mt-12 space-y-2">
                <p class="text-zinc-500 font-bold uppercase tracking-[1em] text-[10px]">Student Council 2026</p>
                <div class="h-[1px] w-40 bg-gradient-to-r from-transparent via-red-600 to-transparent mx-auto"></div>
            </div>
        </div>
    </section>

    <!-- Candidates -->
    <section class="py-20 px-6 max-w-7xl mx-auto">
        <div class="grid grid-cols-1 md:grid-cols-3 gap-12 items-end">
            <!-- รอง 1 -->
            <div class="reveal-left text-center">
                <div class="relative group">
                    <img src="https://i.postimg.cc/hfYqS2w3/image.jpg" alt="" class="w-full aspect-[4/5] object-cover rounded-3xl grayscale group-hover:grayscale-0 transition-all duration-700 img-mask">
                </div>
                <h3 class="mt-8 text-2xl font-black italic uppercase">นางสาวโชติรส ไทยวังชัยต์</h3>
                <p class="text-red-600 text-[10px] font-black tracking-widest uppercase mt-2">รองประธานพรรคคนที่ 1</p>
            </div>

            <!-- ประธาน -->
            <div class="reveal text-center scale-110 z-10">
                <div class="relative group">
                    <div class="absolute -inset-1 bg-red-600 rounded-[2rem] blur opacity-25 group-hover:opacity-75 transition duration-1000"></div>
                    <img src="https://i.postimg.cc/9zpmjtcQ/image.jpg" alt="" class="relative w-full aspect-[4/5] object-cover rounded-[2rem] border-b-8 border-red-600 shadow-2xl">
                </div>
                <h3 class="mt-10 text-4xl font-black italic uppercase leading-none">นายคิรากร แพไธสง</h3>
                <span class="mt-4 inline-block bg-red-700 text-white px-6 py-1 text-[10px] font-black uppercase tracking-tighter rounded-full">The President</span>
            </div>

            <!-- รอง 2 -->
            <div class="reveal-right text-center">
                <div class="relative group">
                    <img src="https://i.postimg.cc/ftC61CYR/image.jpg" alt="" class="w-full aspect-[4/5] object-cover rounded-3xl grayscale group-hover:grayscale-0 transition-all duration-700 img-mask">
                </div>
                <h3 class="mt-8 text-2xl font-black italic uppercase">นางสาวภัทรประภา พยัคฆมะเริง</h3>
                <p class="text-zinc-500 text-[10px] font-black tracking-widest uppercase mt-2">รองประธานพรรคคนที่ 2</p>
            </div>
        </div>
    </section>

    <!-- Policy Section -->
    <section class="py-32 maroon-gradient rounded-t-[5rem]">
        <div class="max-w-6xl mx-auto px-6">
            <div class="mb-24 flex items-baseline justify-between">
                <h2 class="text-6xl md:text-8xl font-black italic uppercase tracking-tighter">POLICY</h2>
                <span class="text-xs font-black opacity-40 tracking-[0.5em]">01-04</span>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                <!-- 1 วิชาการ -->
                <div class="reveal policy-card p-10 rounded-3xl">
                    <h3 class="text-2xl font-black text-red-500 mb-6 uppercase italic">1) นโยบายด้านวิชาการ</h3>
                    <p class="text-xl font-bold leading-relaxed mb-6">-จัดแข่งตอบปัญหาความรู้รอบด้าน(เป็นทีม)โดยแบ่งเป็น6สายชั้นจัดแบ่งเป็นเดือนละสายชั้นวนกันไป</p>
                    <div class="space-y-2 text-zinc-400 font-bold">
                        <p>ข้อดี-ช่วยให้นักเรียนเสริมทักษะความรู้รอบด้าน</p>
                        <p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;-ช่วยเสริมให้นักเรียนเกิดความสามัคคีกัน</p>
                    </div>
                </div>

                <!-- 2 สันทนาการ -->
                <div class="reveal policy-card p-10 rounded-3xl">
                    <h3 class="text-2xl font-black text-red-500 mb-6 uppercase italic">2) นโยบายด้านสันทนาการ</h3>
                    <div class="text-xl font-bold leading-relaxed space-y-4">
                        <p>-ส่งเสริมกิจกรรมRandom Dance</p>
                        <p>-ประกวดเดินแบบให้กับLGBTQ(โดยเฉพาะ)</p>
                        <p>-เปิดเพจฝากขายเสื้อผ้ามือ2ให้กับพี่ๆน้องๆได้ฝากพวกเราขายได้ทันที</p>
                    </div>
                </div>

                <!-- 3 Social -->
                <div class="reveal policy-card p-10 rounded-3xl md:col-span-2">
                    <h3 class="text-2xl font-black text-red-500 mb-6 uppercase italic">3) นโยบายด้านSocial</h3>
                    <div class="text-lg font-bold leading-relaxed space-y-6">
                        <p>-ส่งเสริมLGBTQแบบเต็มที่เพื่อไม่ให้เกิดการแบ่งแยกและBullyingกันในสังคม ผ่านกิจกรรมเดินแบบหรือประกวดความสวยงามในตัวเราเผื่อสร้างความมั่นใจให้ตัวเองตามหัวข้อนโยบายด้านสันทนาการ (ผู้ที่สนใจประกวดไม่ว่าจะเพศใดก็สามารถลงประกวดได้เช่นกัน)</p>
                        <div class="h-[1px] bg-white/10 w-full"></div>
                        <p>-กล่องระบายความคิดเห็นความรู้สึกหรือปัญหาของโรเรียน</p>
                        <div class="h-[1px] bg-white/10 w-full"></div>
                        <p>-กิจกรรมกระชับความสัมพันธ์พี่-น้องพี่ๆน้องที่เครียดจากการเรียนหรือน้องๆที่จะขึ้นเรียนต่อในสายชั้นม.4แต่ไม่รู้ว่าจะเรียนสายไหนสามารถทักสอบถามได้ทันทีทางแอคห้องIGหรือสอบถามโดยตรงจากพี่ในพรรคได้เลย</p>
                    </div>
                </div>

                <!-- 4 สุขอนามัย -->
                <div class="reveal policy-card p-10 rounded-3xl md:col-span-2 border-red-600/50 bg-black">
                    <h3 class="text-2xl font-black text-red-500 mb-8 uppercase italic underline decoration-red-600 underline-offset-8">4) นโยบายด้านสุขอนามัยและอุปโภค</h3>
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-10 text-lg font-bold">
                        <div class="space-y-6">
                            <p>-ใช้ผลิตภัณฑ์จากธรรมชาติมาช่วยดับกลิ่นไม่พึงประสงค์ในห้องน้ำเช่น มะกรูด ตะไคร้โดยจะเปลี่ยนทุก1อาทิตย์</p>
                            <p>-มียาประจำแต่ละอาคารทุกอาคารเวลาเกิดเหตุฉุกเฉิน</p>
                            <p class="text-red-500 text-sm font-black italic">-ข้อดี:ทำให้สดวกขึ้นเวลาเกิดเหตุฉุกเฉินต่างๆ</p>
                        </div>
                        <div class="space-y-6">
                            <p>-มีผ้าอนามัยฟรีพร้อมกระดาษห่อทิ้งถังขยะสะดวกต่อผู้ที่จำเป็นต้องใช้</p>
                            <p>-มีการเดินตรวจโต๊ะสำหรับการเรียนเพื่อตรวจหาจำนวนที่ชำรุดแล้วนำไปแจ้งแก้ไข้ทันที</p>
                            <p class="text-red-500 text-sm font-black italic">ข้อดี :จะทำให้โต้ะของโรงเรียนชำรุดน้อยลงและไม่ทำให้เกิดอันตราย</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="py-40 text-center relative overflow-hidden">
        <div class="reveal">
            <h2 class="hero-title opacity-10 absolute left-1/2 -translate-x-1/2 -top-10 select-none">VOTE NOW</h2>
            <h2 class="text-4xl font-black italic uppercase mb-12">Vote <span class="text-red-600">moveforwardpaty</span></h2>
            <div class="flex justify-center gap-12 mb-20">
                <a href="https://www.instagram.com/moveforwardpaty.pm" target="_blank" class="hover:text-red-600 transition-transform hover:scale-125"><i data-lucide="instagram" class="w-8 h-8"></i></a>
                <a href="https://www.tiktok.com/@moveforwardpaty" target="_blank" class="hover:text-red-600 transition-transform hover:scale-125">
                    <svg class="w-8 h-8 fill-current" viewBox="0 0 24 24"><path d="M12.525.02c1.31-.02 2.61-.01 3.91-.02.08 1.53.63 3.09 1.75 4.17 1.12 1.11 2.7 1.62 4.24 1.79v4.03c-1.44-.17-2.89-.6-4.14-1.32-.09 4-1.23 7.74-4.44 10.32-2.72 2.26-6.56 3.06-9.86 2.05-3.3-1.02-5.74-3.92-6.51-7.24-.8-3.41.36-7.3 3-9.76 2.31-2.15 5.86-2.9 8.87-1.78.03.81.02 1.62.03 2.43-1.61-.41-3.41-.16-4.76.87-1.35 1.02-1.95 2.87-1.52 4.54.4 1.57 1.83 2.8 3.4 3.05 1.62.24 3.3-.3 4.28-1.63.85-1.16 1.05-2.65 1.05-4.04V.02z"/></svg>
                </a>
            </div>
            <p class="text-[8px] font-black uppercase tracking-[2em] opacity-20">The Future is Maroon & Black</p>
        </div>
    </footer>

    <script>
        lucide.createIcons();
        ScrollReveal().reveal('.reveal', { delay: 200, distance: '50px', origin: 'bottom', duration: 1000 });
        ScrollReveal().reveal('.reveal-left', { delay: 400, distance: '50px', origin: 'left', duration: 1000 });
        ScrollReveal().reveal('.reveal-right', { delay: 400, distance: '50px', origin: 'right', duration: 1000 });
    </script>
</body>
</html>

