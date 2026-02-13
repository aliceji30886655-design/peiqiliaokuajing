<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>跨境电商全平台招商与培训中心</title>
    <style>
        /* --- 1. 全局样式重置 --- */
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'PingFang SC', 'Microsoft YaHei', sans-serif; }
        body { background-color: #f4f6f9; color: #333; line-height: 1.6; }
        a { text-decoration: none; color: inherit; }
        ul { list-style: none; }

        /* --- 2. 导航栏 --- */
        header { background: #fff; box-shadow: 0 2px 10px rgba(0,0,0,0.05); position: sticky; top: 0; z-index: 100; }
        .nav-container { max-width: 1200px; margin: 0 auto; display: flex; justify-content: space-between; align-items: center; padding: 15px 20px; }
        .logo { font-size: 24px; font-weight: bold; color: #0056b3; }
        .nav-menu a { margin-left: 20px; color: #555; font-weight: 500; transition: color 0.3s; }
        .nav-menu a:hover { color: #0056b3; }
        .btn-cta { background: #0056b3; color: #fff !important; padding: 8px 20px; border-radius: 20px; }

        /* --- 3. 首屏 Banner (Hero Section) --- */
        .hero { 
            background: linear-gradient(135deg, #0056b3 0%, #00c6ff 100%); 
            color: #fff; text-align: center; padding: 80px 20px; 
        }
        .hero h1 { font-size: 2.5rem; margin-bottom: 15px; }
        .hero p { font-size: 1.2rem; opacity: 0.9; margin-bottom: 30px; }
        .hero-btn { background: #ff9900; color: #fff; padding: 12px 30px; border-radius: 5px; font-weight: bold; font-size: 1.1rem; border: none; cursor: pointer; }
        
        /* --- 4. 核心业务板块 (Grid布局) --- */
        .section { max-width: 1200px; margin: 50px auto; padding: 0 20px; }
        .section-title { text-align: center; font-size: 2rem; margin-bottom: 40px; color: #222; position: relative; }
        .section-title::after { content: ''; display: block; width: 60px; height: 3px; background: #0056b3; margin: 10px auto; }
        
        .services-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 20px; }
        .service-card { background: #fff; padding: 30px; border-radius: 10px; text-align: center; transition: transform 0.3s; box-shadow: 0 5px 15px rgba(0,0,0,0.05); }
        .service-card:hover { transform: translateY(-5px); }
        .icon { font-size: 40px; margin-bottom: 15px; display: block; }
        .service-card h3 { margin-bottom: 10px; color: #0056b3; }
        
        /* --- 5. 课程表 (Table样式) --- */
        .schedule-table { width: 100%; border-collapse: collapse; background: #fff; box-shadow: 0 5px 15px rgba(0,0,0,0.05); border-radius: 10px; overflow: hidden; }
        .schedule-table th, .schedule-table td { padding: 15px; text-align: left; border-bottom: 1px solid #eee; }
        .schedule-table th { background: #f8f9fa; color: #0056b3; font-weight: bold; }
        .schedule-table tr:last-child td { border-bottom: none; }
        .tag { display: inline-block; padding: 4px 10px; border-radius: 4px; font-size: 12px; color: #fff; }
        .tag-hot { background: #ff4d4f; }
        .tag-new { background: #52c41a; }

        /* --- 6. 联系我们 & 底部 --- */
        .contact-section { background: #fff; text-align: center; padding: 60px 20px; margin-top: 50px; }
        .contact-box { border: 2px dashed #0056b3; display: inline-block; padding: 30px 50px; border-radius: 10px; background: #f0f7ff; }
        .phone-number { font-size: 2rem; font-weight: bold; color: #0056b3; margin: 10px 0; display: block; }
        footer { background: #333; color: #aaa; text-align: center; padding: 20px; margin-top: 0; }

        /* --- 7. 移动端适配 --- */
        @media (max-width: 768px) {
            .nav-menu { display: none; } /* 手机端隐藏导航菜单，简化展示 */
            .hero h1 { font-size: 1.8rem; }
            .schedule-table th, .schedule-table td { padding: 10px; font-size: 14px; }
            .contact-box { padding: 20px; width: 100%; }
            .phone-number { font-size: 1.5rem; }
        }
    </style>
</head>
<body>

    <header>
        <div class="nav-container">
            <div class="logo">🚀 跨境出海服务</div>
            <nav class="nav-menu">
                <a href="#services">平台入驻</a>
                <a href="#courses">培训课表</a>
                <a href="#design">美工设计</a>
                <a href="#contact" class="btn-cta">联系佩琪</a>
            </nav>
        </div>
    </header>

    <section class="hero">
        <h1>2026年 跨境电商全平台招商启动</h1>
        <p>覆盖亚马逊本土、BOL、OTTO、Target、TikTok等主流平台</p>
        <button class="hero-btn" onclick="scrollToContact()">立即获取入驻名额</button>
    </section>

    <section id="services" class="section">
        <h2 class="section-title">核心业务服务</h2>
        <div class="services-grid">
            <div class="service-card">
                <span class="icon">🛒</span>
                <h3>平台入驻代办</h3>
                <p>亚马逊本土店、OTTO、Target、Leroy Merlin 绿色通道下店。</p>
            </div>
            <div class="service-card">
                <span class="icon">📱</span>
                <h3>TikTok 运营</h3>
                <p>TikTok TOB 运营、直播带货、短视频引流全案策划。</p>
            </div>
            <div class="service-card">
                <span class="icon">🎨</span>
                <h3>电商美工设计</h3>
                <p>亚马逊主图精修、A+页面设计、品牌Logo、AI 智能做图。</p>
            </div>
            <div class="service-card">
                <span class="icon">📦</span>
                <h3>独立站建站</h3>
                <p>Shopify 独立站搭建、Google SEO 优化引流服务。</p>
            </div>
        </div>
    </section>

    <section id="courses" class="section">
        <h2 class="section-title">2月实战课表安排</h2>
        <table class="schedule-table">
            <thead>
                <tr>
                    <th>课程名称</th>
                    <th>开课时间</th>
                    <th>状态</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>美客多 (Mercado Libre) 掘金特训营</td>
                    <td>2月1日 - 2月2日</td>
                    <td><span class="tag tag-new">报名中</span></td>
                </tr>
                <tr>
                    <td>TikTok 直播与短视频实战</td>
                    <td>2月5日 - 2月8日</td>
                    <td><span class="tag tag-hot">热门</span></td>
                </tr>
                <tr>
                    <td>Google SEO 独立站引流课</td>
                    <td>2月5日 - 2月8日</td>
                    <td><span class="tag tag-new">余位不多</span></td>
                </tr>
                <tr>
                    <td>Shopify 独立站建站全解</td>
                    <td>2月5日 - 2月8日</td>
                    <td><span class="tag tag-new">报名中</span></td>
                </tr>
            </tbody>
        </table>
    </section>

    <section id="design" class="section" style="background: #fff; padding: 40px; border-radius: 10px;">
        <h2 class="section-title">亚马逊主图设计服务</h2>
        <p style="text-align: center; margin-bottom: 20px;">
            我们提供专业的亚马逊主图、A+页面设计，结合 AI 技术快速出图，提升点击率 (CTR)。
        </p>
        <div style="text-align: center; color: #888; background: #eee; padding: 40px; border-radius: 8px;">
            [ 此处可插入你的设计案例作品集图片 ]
        </div>
    </section>

    <section id="contact" class="contact-section">
        <h2>立即咨询 & 报名</h2>
        <p>专业顾问一对一解答，协助您布局全球市场</p>
        <br>
        <div class="contact-box">
            <p>联系人：佩琪 (Peggy)</p>
            <a href="tel:13760280059" class="phone-number">13760280059</a>
            <p style="font-size: 0.9rem; color: #666;">(点击电话号码即可拨打)</p>
        </div>
    </section>

    <footer>
        <p>© 2026 跨境电商服务中心 All Rights Reserved.</p>
    </footer>

    <script>
        // 简单的平滑滚动效果
        function scrollToContact() {
            document.getElementById('contact').scrollIntoView({ behavior: 'smooth' });
        }
    </script>
</body>
</html>
