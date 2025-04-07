<!DOCTYPE html>
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
    background-color: #4CAF50;
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

/* 响应式布局 */
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
    <!-- 时间轴项1 -->
    <div class="timeline-item left">
        <div class="timeline-content">
            <h3>2023年1月</h3>
            <p>项目启动</p>
        </div>
    </div>

    <!-- 时间轴项2 -->
    <div class="timeline-item right">
        <div class="timeline-content">
            <h3>2023年3月</h3>
            <p>第一阶段完成</p>
        </div>
    </div>

    <!-- 时间轴项3 -->
    <div class="timeline-item left">
        <div class="timeline-content">
            <h3>2023年6月</h3>
            <p>产品发布</p>
        </div>
    </div>
</div>

</body>
</html>
