<!-- <!DOCTYPE html> -->
<html>
<head>
<style>
.timeline {
    position: relative;
    max-width: 1200px;
    margin: 0 auto;
}

<!-- /* 时间轴竖线 */ -->
.timeline::after {
    content: '';
    position: absolute;
    width: 6px;
    background-color:rgb(160, 160, 160);
    top: 0;
    bottom: 0;
    left: 50%;
    margin-left: -3px;
}

<!-- /* 时间轴容器 */ -->
.timeline-item {
    padding: 10px 40px;
    position: relative;
    background-color: inherit;
    width: 50%;
}

<!-- /* 时间轴内容框 */ -->
.timeline-content {
    padding: 20px 30px;
    background-color: white;
    position: relative;
    border-radius: 6px;
    border: 1px solid #ddd;
    box-shadow: 0 2px 4px rgba(0,0,0,0.1);
}

<!-- /* 左侧对齐 */ -->
.left {
    left: 0;
}

<!-- /* 右侧对齐 */ -->
.right {
    left: 50%;
}

<!-- /* 时间轴圆点 */ -->
.timeline-item::after {
    content: '';
    position: absolute;
    width: 25px;
    height: 25px;
    right: -12px;
    background-color: white;
    border: 4px solid #000000;
    top: 15px;
    border-radius: 50%;
    z-index: 1;
}

.right::after {
    left: -12px;
}

<!-- /* 响应式布局 */ -->
@media screen and (max-width: 600px) {
    .timeline::after {
        left: 31px;
    }

    .timeline-item {
        width: 100%;
        padding-left: 70px;
        padding-right: 25px;
    }

    .timeline-item::before {
        left: 60px;
    }

    .left::after, .right::after {
        left: 15px;
    }

    .right {
        left: 0%;
    }
}
</style>
</head>
<body>

<div class="timeline">

    <div class="timeline-item left">
        <div class="timeline-content">
            <h3>2001年7月4日</h3>
            <p>地球Online（困难模式）开局</p>
        </div>
    </div>

    <div class="timeline-item right">
        <div class="timeline-content">
            <h3>2005年</h3>
            <p>从艺（小提琴）</p>
        </div>
    </div>

    <div class="timeline-item left">
        <div class="timeline-content">
            <h3>2007年9月</h3>
            <p>小学：吉林市船营区第四小学</p>
        </div>
    </div>

    <div class="timeline-item right">
        <div class="timeline-content">
            <h3>2008年</h3>
            <p>发现不喜欢小提琴，开始学声乐</p>
        </div>
    </div>

    <div class="timeline-item left">
        <div class="timeline-content">
            <h3>2009年</h3>
            <p>接触戏曲，开始自学</p>
        </div>
    </div>

    <div class="timeline-item right">
        <div class="timeline-content">
            <h3>2010年</h3>
            <p>前往中国人民解放军艺术学院（现中国人民解放军国防大学军事文化学院）公费学习“程派”青衣</p>
        </div>
    </div>

    <div class="timeline-item left">
        <div class="timeline-content">
            <h3>2011年</h3>
            <p>尝试组建乐队，无果</p>
        </div>
    </div>

    <div class="timeline-item right">
        <div class="timeline-content">
            <h3>2012年</h3>
            <p>尝试组建乐团：末日乐园（逸衡馆前身）</p>
        </div>
    </div>

    <div class="timeline-item left">
        <div class="timeline-content">
            <h3>2013年初</h3>
            <p>“末日乐园”更名“逸衡馆”，以第一次商演作为乐团的起点</p>
        </div>
    </div>

    <div class="timeline-item right">
        <div class="timeline-content">
            <h3>2013年9月</h3>
            <p>吉林市第五中学分校（现：吉林市亚桥中学）</p>
        </div>
    </div>

    <div class="timeline-item left">
        <div class="timeline-content">
            <h3>2014年</h3>
            <p>因变声不善，转行古典美声</p>
            <p>从艺所得一口气充了1000Q币</p>
            <p>受邀赴韩务工于 Big Hit Entertainment（빅히트 엔터테인먼트，现为HYBE (하이브) Corporation）</p>
        </div>
    </div>

    <div class="timeline-item right">
        <div class="timeline-content">
            <h3>2015年初</h3>
            <p>无力学艺，开始学习文化课，发现数学的乐趣</p>
        </div>
    </div>

    <div class="timeline-item left">
        <div class="timeline-content">
            <h3>2016年9月</h3>
            <p>高中：吉林毓文中学</p>
            <p>第一次月考喜提年级第四，除实验班年级第一</p>
        </div>
    </div>

    <div class="timeline-item right">
        <div class="timeline-content">
            <h3>2017年</h3>
            <p>好好学习（装文化人）</p>
        </div>
    </div>

    <div class="timeline-item left">
        <div class="timeline-content">
            <h3>2018年3月</h3>
            <p>合伙开了吉林市前几家剧本杀之一</p>
        </div>
    </div>

    <div class="timeline-item right">
        <div class="timeline-content">
            <h3>2019年9月</h3>
            <p>大学本科：深圳大学（统计学）</p>
        </div>
    </div>

    <div class="timeline-item left">
        <div class="timeline-content">
            <h3>2019年11月</h3>
            <p>在延吉合伙开了家酒吧（别问叫啥，8个月就黄了）</p>
        </div>
    </div>

    <div class="timeline-item right">
        <div class="timeline-content">
            <h3>2020年2月</h3>
            <p>“逸衡馆”的大家忙各自的事业，就地解散</p>
        </div>
    </div>

    <div class="timeline-item left">
        <div class="timeline-content">
            <h3>2020年4月4日</h3>
            <p>无情的COVID-19和他的既往病史带走了他的生命，也带走了我的部分灵魂，喜提抑郁症</p>
        </div>
    </div>

    <div class="timeline-item left">
        <div class="timeline-content">
            <h3>2021年</h3>
            <p>抑郁</p>
        </div>
    </div>

    <div class="timeline-item right">
        <div class="timeline-content">
            <h3>2022年</h3>
            <p>治疗至今，开始停药，暂不复发</p>
        </div>
    </div>

    <div class="timeline-item left">
        <div class="timeline-content">
            <h3>2023年上半年</h3>
            <p>考研失败</p>
            <p>雅思失败</p>
            <p>申硕失败</p>
        </div>
    </div>

    <div class="timeline-item right">
        <div class="timeline-content">
            <h3>2023年6月</h3>
            <p>本科毕业</p>
            <p>理学学士（数学与应用数学专业）</p>
            <p>经济学学士（金融学专业）</p>
        </div>
    </div>

    <div class="timeline-item left">
        <div class="timeline-content">
            <h3>2023年9月</h3>
            <p>入职吉林市某教培机构</p>
        </div>
    </div>

    <div class="timeline-item right">
        <div class="timeline-content">
            <h3>2024年1月</h3>
            <p>兼职某留学辅导机构</p>
        </div>
    </div>

    <div class="timeline-item left">
        <div class="timeline-content">
            <h3>2024年9月</h3>
            <p>硕士：英国格拉斯哥大学（统计学）</p>
        </div>
    </div>

    <div class="timeline-item right">
        <div class="timeline-content">
            <h3>2024年10月</h3>
            <p>入职路觅教育</p>
        </div>
    </div>

    <div class="timeline-item left">
        <div class="timeline-content">
            <h3>2025年9月</h3>
            <p>访问学者：西交利物浦大学</p>
        </div>
    </div>

    <div class="timeline-item right">
        <div class="timeline-content">
            <h3>2024年11月</h3>
            <p>硕士毕业</p>
            <p>理学硕士（统计学专业）</p>
        </div>
    </div>

    <div class="timeline-item left">
        <div class="timeline-content">
            <h3>2026年1月</h3>
            <p>博士：西交利物浦大学</p>
        </div>
    </div>

    <div class="timeline-item right">
        <div class="timeline-content">
            <h3>预计2029年1月</h3>
            <p>博士毕业</p>
            <p>哲学博士（数学专业）</p>
        </div>
    </div>
    
</div>

</body>
</html>
