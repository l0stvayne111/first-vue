<template>
  <!--    <div class="card">-->
  <!--        <div class="card-header">-->
  <!--            <h5 class="card-title">{{ title }}</h5>-->
  <!--            <h6 class="card-subtitle mb-2 text-muted">{{user}}</h6>-->
  <!--        </div>-->
  <!--        <div class="card-body">-->
  <!--            <p class="card-text">{{ description }}</p>-->
  <!--        </div>-->
  <!--        <div class="card-footer text-muted">{{ date }}</div>-->
  <!--    </div>-->


    <div class="card">
        <div class="card-header">
            <div class="card-user">
                {{ name }}
            </div>
            <div class="card-date">
                {{ date }}
            </div>
        </div>
        <div class="card-body">
          <div class="card-title">{{title}}</div>
            <div class="card-description">{{description}}</div>
        </div>
        <div class="card-footer">
            <router-link class="card-link" :to="`/post/${id}`">
                Читать далее
            </router-link>
        </div>
    </div>
</template>

<script>
export default {
    name: "BlogCard",
    props: {
        id: Intl,
        title: String,
        description: String,
        date: String,
        name: String
    }
}
</script>

<style scoped>
.card {
    display: block;
    padding: 24px 0 32px 0;
    text-align: left;

    border-top: 1px solid #eee;
}

.card-header {
    display: flex;
    align-items: center;
}

.card-user,
.card-date {
    font-size: 14px;

}

.card-user {
    color: #000;
}

.card-date {
    color: #a9a9a9;
    margin-left: 12px;
}

.card-body {
    padding: 8px 0;
}
.card-title {
    font-size: 20px;
    font-weight: 700;
    color: #2c3e50;
    margin-bottom: 12px;
}
.card-description {
    font-size: 16px;
    line-height: 1.2;
    color: #bbbaba;
}

.card-footer {

}
.card-link {
    color: #1e87f0;
    font-size: 14px;
    text-decoration: none;
}
</style>