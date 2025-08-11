<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>实验室新闻</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            min-height: 100vh;
            padding: 20px;
            line-height: 1.6;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
        }

        .page-header {
            text-align: center;
            margin-bottom: 40px;
            padding: 20px;
        }

        .page-title {
            font-size: 2.5rem;
            color: #2c3e50;
            margin-bottom: 10px;
            font-weight: 700;
        }

        .page-subtitle {
            font-size: 1.1rem;
            color: #7f8c8d;
            font-weight: 400;
        }

        .news-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 30px;
            padding: 20px 0;
        }

        .news-card {
            background: white;
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
            overflow: hidden;
            transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            cursor: pointer;
            height: 420px;
            display: flex;
            flex-direction: column;
        }

        .news-card:hover {
            transform: translateY(-10px) scale(1.02);
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.15);
        }

        .card-header {
            padding: 20px 20px 15px;
            border-bottom: 1px solid #f8f9fa;
        }

        .card-icon {
            font-size: 1.5rem;
            margin-right: 10px;
        }

        .card-title {
            font-size: 1.3rem;
            font-weight: 600;
            color: #2c3e50;
            display: flex;
            align-items: center;
            margin-bottom: 8px;
        }

        .card-date {
            font-size: 0.9rem;
            color: #95a5a6;
            font-weight: 500;
        }

        .card-content {
            flex: 1;
            padding: 20px;
            display: flex;
            flex-direction: column;
        }

        .card-image {
            width: 100%;
            height: 160px;
            object-fit: cover;
            border-radius: 8px;
            margin-bottom: 15px;
            transition: transform 0.3s ease;
        }

        .news-card:hover .card-image {
            transform: scale(1.05);
        }

        .card-description {
            color: #5a6c7d;
            font-size: 0.95rem;
            line-height: 1.6;
            flex: 1;
        }

        .card-tags {
            display: flex;
            gap: 8px;
            margin-top: 15px;
            flex-wrap: wrap;
        }

        .tag {
            background: linear-gradient(45deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 4px 12px;
            border-radius: 20px;
            font-size: 0.8rem;
            font-weight: 500;
        }

        .welcome .card-title { color: #e74c3c; }
        .welcome .card-header { background: linear-gradient(45deg, #ff9a9e 0%, #fecfef 100%); }

        .bbq .card-title { color: #f39c12; }
        .bbq .card-header { background: linear-gradient(45deg, #ffecd2 0%, #fcb69f 100%); }

        .career .card-title { color: #3498db; }
        .career .card-header { background: linear-gradient(45deg, #a8edea 0%, #fed6e3 100%); }

        .card-footer {
            padding: 15px 20px;
            background: #f8f9fa;
            border-top: 1px solid #e9ecef;
        }

        .read-more {
            color: #667eea;
            text-decoration: none;
            font-weight: 600;
            font-size: 0.9rem;
            transition: color 0.3s ease;
        }

        .read-more:hover {
            color: #764ba2;
        }

        @media (max-width: 768px) {
            .news-grid {
                grid-template-columns: 1fr;
                gap: 20px;
            }
            
            .page-title {
                font-size: 2rem;
            }
            
            .news-card {
                height: auto;
                min-height: 400px;
            }
        }

        /* Loading animation */
        .news-card {
            animation: fadeInUp 0.6s ease-out forwards;
            opacity: 0;
            transform: translateY(30px);
        }

        .news-card:nth-child(1) { animation-delay: 0.1s; }
        .news-card:nth-child(2) { animation-delay: 0.2s; }
        .news-card:nth-child(3) { animation-delay: 0.3s; }

        @keyframes fadeInUp {
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="page-header">
            <h1 class="page-title">实验室新闻</h1>
            <p class="page-subtitle">记录我们的精彩时刻与重要活动</p>
        </div>

        <div class="news-grid">
            <!-- 迎新活动卡片 -->
            <div class="news-card welcome">
                <div class="card-header">
                    <h3 class="card-title">
                        <span class="card-icon">🎉</span>
                        实验室迎新活动：携手新程
                    </h3>
                    <div class="card-date">2024年9月</div>
                </div>
                <div class="card-content">
                    <img src="data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMzIwIiBoZWlnaHQ9IjE2MCIgdmlld0JveD0iMCAwIDMyMCAxNjAiIGZpbGw9Im5vbmUiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+CjxyZWN0IHdpZHRoPSIzMjAiIGhlaWdodD0iMTYwIiBmaWxsPSIjRkY5QTlFIi8+CjxjaXJjbGUgY3g9IjE2MCIgY3k9IjgwIiByPSI0MCIgZmlsbD0iI0ZGRiIvPgo8dGV4dCB4PSIxNjAiIHk9Ijg1IiB0ZXh0LWFuY2hvcj0ibWlkZGxlIiBmaWxsPSIjRkY5QTlFIiBmb250LWZhbWlseT0iQXJpYWwiIGZvbnQtc2l6ZT0iMTQiPuasoOi/juiBmmk8L3RleHQ+Cjx0ZXh0IHg9IjE2MCIgeT0iMTMwIiB0ZXh0LWFuY2hvcj0ibWlkZGxlIiBmaWxsPSIjRkZGIiBmb250LWZhbWlseT0iQXJpYWwiIGZvbnQtc2l6ZT0iMTYiPuaWsOeUn-S4juW4iOWFhOW4iOWnkOWQjOWcqOS6pOa1gTwvdGV4dD4KPC9zdmc+" 
                         alt="迎新聚餐" class="card-image">
                    <p class="card-description">
                        欢迎新同学加入实验室大家庭！通过轻松愉快的聚餐交流，帮助新生快速融入团队。新生与师兄师姐围坐交流，共享美食，促进师兄师姐与新生的交流。
                    </p>
                    <div class="card-tags">
                        <span class="tag">团队建设</span>
                        <span class="tag">新生欢迎</span>
                    </div>
                </div>
                <div class="card-footer">
                    <a href="#" class="read-more">了解更多 →</a>
                </div>
            </div>

            <!-- 烧烤活动卡片 -->
            <div class="news-card bbq">
                <div class="card-header">
                    <h3 class="card-title">
                        <span class="card-icon">🍖</span>
                        东湖烧烤野餐活动
                    </h3>
                    <div class="card-date">2024年春秋两季</div>
                </div>
                <div class="card-content">
                    <img src="data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMzIwIiBoZWlnaHQ9IjE2MCIgdmlld0JveD0iMCAwIDMyMCAxNjAiIGZpbGw9Im5vbmUiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+CjxyZWN0IHdpZHRoPSIzMjAiIGhlaWdodD0iMTYwIiBmaWxsPSIjRkZFQ0QyIi8+CjxyZWN0IHg9IjEwMCIgeT0iNjAiIHdpZHRoPSIxMjAiIGhlaWdodD0iNDAiIGZpbGw9IiM4QjQ1MTMiLz4KPGV4bGlwc2UgY3g9IjE2MCIgY3k9IjUwIiByeD0iMzAiIHJ5PSIxMCIgZmlsbD0iI0ZGNjcwMCIvPgo8dGV4dCB4PSIxNjAiIHk9IjEzMCIgdGV4dC1hbmNob3I9Im1pZGRsZSIgZmlsbD0iI0ZGNjcwMCIgZm9udC1mYW1pbHk9IkFyaWFsIiBmb250LXNpemU9IjE0Ij7kuJzmuZbngKfng6nnvZTnnYjmtLo8L3RleHQ+Cjx0ZXh0IHg9IjE2MCIgeT0iMTQ1IiB0ZXh0LWFuY2hvcj0ibWlkZGxlIiBmaWxsPSIjOEI0NTEzIiBmb250LWZhbWlseT0iQXJpYWwiIGZvbnQtc2l6ZT0iMTIiPuWunOWxlua4uOaIj+OAgeeul-aJiOWQiOS9nO+8jOWinuWKoOe+jumjn+OAgeasoOi/juWdmei1jjwvdGV4dD4KPC9zdmc+" 
                         alt="东湖烧烤" class="card-image">
                    <p class="card-description">
                        年度团建活动，包含湖边烧烤、团队游戏与东湖散步，增进团队凝聚力。同学们分工合作准备食材和烧烤，在欢声笑语中圆满结束，大家期待下次再聚！
                    </p>
                    <div class="card-tags">
                        <span class="tag">团队游戏</span>
                        <span class="tag">户外烧烤</span>
                        <span class="tag">湖边散步</span>
                    </div>
                </div>
                <div class="card-footer">
                    <a href="#" class="read-more">查看活动相册 →</a>
                </div>
            </div>

            <!-- 求职分享会卡片 -->
            <div class="news-card career">
                <div class="card-header">
                    <h3 class="card-title">
                        <span class="card-icon">🚀</span>
                        研三求职经验分享会
                    </h3>
                    <div class="card-date">2024年10月</div>
                </div>
                <div class="card-content">
                    <img src="data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMzIwIiBoZWlnaHQ9IjE2MCIgdmlld0JveD0iMCAwIDMyMCAxNjAiIGZpbGw9Im5vbmUiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+CjxyZWN0IHdpZHRoPSIzMjAiIGhlaWdodD0iMTYwIiBmaWxsPSIjQThFREVBIi8+CjxyZWN0IHg9IjUwIiB5PSI0MCIgd2lkdGg9IjIyMCIgaGVpZ2h0PSI4MCIgZmlsbD0iI0ZGRiIgc3Ryb2tlPSIjMzQ5OERCIiBzdHJva2Utd2lkdGg9IjIiLz4KPGV4bGlwc2UgY3g9IjEwMCIgY3k9IjgwIiByeD0iMTUiIHJ5PSIyMCIgZmlsbD0iIzM0OThEQiIvPgo8dGV4dCB4PSIxNjAiIHk9Ijg1IiB0ZXh0LWFuY2hvcj0ibWlkZGxlIiBmaWxsPSIjMzQ5OERCIiBmb250LWZhbWlseT0iQXJpYWwiIGZvbnQtc2l6ZT0iMTQiPuWwsOS8muWIhuS6q+mbtui+hTwvdGV4dD4KPHR4dCB4PSIxNjAiIHk9IjEzNSIgdGV4dC1hbmNob3I9Im1pZGRsZSIgZmlsbD0iIzM0OThEQiIgZm9udC1mYW1pbHk9IkFyaWFsIiBmb250LXNpemU9IjEyIj7miJDlip/lhaXogYzlsI_nsbPjgIHkuK3lu7rkuInlsYDnrYnnrYnlhazlj7g8L3RleHQ+Cjx0ZXh0IHg9IjE2MCIgeT0iMTUwIiB0ZXh0LWFuY2hvcj0ibWlkZGxlIiBmaWxsPSIjMzQ5OERCIiBmb250LWZhbWlseT0iQXJpYWwiIGZvbnQtc2l6ZT0iMTIiPumHjeW6puS6kuiBlOe9kS/lm73kvIEvpbC46L2m562J6KGM5Lia5YiG5LqrPC90ZXh0Pgo8L3N2Zz4=" 
                         alt="求职分享会" class="card-image">
                    <p class="card-description">
                        为帮助研三同学把握秋招黄金期，特邀已经毕业入职小米、中建三局等公司校友开展深度分享，覆盖互联网/国企/通信等行业，助力师弟师妹拿到心仪offer。
                    </p>
                    <div class="card-tags">
                        <span class="tag">求职指导</span>
                        <span class="tag">校友分享</span>
                        <span class="tag">面试技巧</span>
                    </div>
                </div>
                <div class="card-footer">
                    <a href="#" class="read-more">观看回放 →</a>
                </div>
            </div>
        </div>
    </div>

    <script>
        // 添加交互效果
        document.addEventListener('DOMContentLoaded', function() {
            const cards = document.querySelectorAll('.news-card');
            
            cards.forEach(card => {
                card.addEventListener('mouseenter', function() {
                    this.style.zIndex = '10';
                });
                
                card.addEventListener('mouseleave', function() {
                    this.style.zIndex = '1';
                });
                
                // 点击卡片效果
                card.addEventListener('click', function() {
                    const ripple = document.createElement('div');
                    ripple.style.position = 'absolute';
                    ripple.style.borderRadius = '50%';
                    ripple.style.background = 'rgba(255, 255, 255, 0.6)';
                    ripple.style.transform = 'scale(0)';
                    ripple.style.animation = 'ripple 0.6s linear';
                    ripple.style.left = '50%';
                    ripple.style.top = '50%';
                    ripple.style.width = '20px';
                    ripple.style.height = '20px';
                    ripple.style.marginLeft = '-10px';
                    ripple.style.marginTop = '-10px';
                    
                    this.style.position = 'relative';
                    this.appendChild(ripple);
                    
                    setTimeout(() => {
                        ripple.remove();
                    }, 600);
                });
            });
        });
        
        // 添加波纹动画
        const style = document.createElement('style');
        style.textContent = `
            @keyframes ripple {
                to {
                    transform: scale(4);
                    opacity: 0;
                }
            }
        `;
        document.head.appendChild(style);
    </script>
</body>
</html>
