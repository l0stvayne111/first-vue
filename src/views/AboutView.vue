<template>
    <div class="about">
        <div class="user">
            <div class="user-avatar">
                <img src="https://sun9-23.userapi.com/impg/1lrY4PY_dgyOKa1p5iwMVKu5FZAfA24rvp50xg/M9exp2Uz6mk.jpg?size=1072x1080&quality=95&sign=e7f9e9b7c935153eb7aef54e8cb5d834&type=album" alt="">
            </div>
            <div class="user-name">
                Евгения Скуратова
            </div>
            <div class="user-status">
                UI/UX Designer
            </div>
            <div class="user-description">
                Lorem ipsum dolor sit amet, consectetur adipisicing elit. Distinctio earum reprehenderit sapiente vel.
                Accusamus alias amet at dignissimos dolorum earum eveniet explicabo id impedit incidunt ipsam laudantium
                libero minus nam nesciunt omnis pariatur placeat porro possimus quidem sed suscipit temporibus tenetur,
                vitae voluptas! Corporis, dolore maiores rerum tempora veniam voluptatum?
            </div>
        </div>
    </div>
</template>


<style>
.about {
    max-width: 1200px;
    margin: 0 auto;
    width: 100%;
}


.user {
    position: relative;
    text-align: center;
    margin-top: 48px;
}

.user-avatar {
    width: 150px;
    height: 150px;
    border-radius: 50%;
    background: #1e87f0;
    display: inline-block;
    overflow: hidden;

}

.user-avatar img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

.user-name {
    color: #2c3e50;
    font-size: 24px;
    font-weight: 700;
    line-height: 1;
    margin: 12px 0 6px 0;
}

.user-status {
    font-size: 16px;
    color: #bbbaba;
    font-weight: 500;
}

.user-description {
    font-size: 14px;
    color: #2c3e50;
    line-height: 1.4;
    text-align: justify;
    max-width: 600px;
    width: 100%;
    margin: 12px auto;
}
</style>