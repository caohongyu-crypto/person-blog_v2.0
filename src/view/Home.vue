<template>
  <div class="home">
    <el-container>
      <!-- 头部内容区域 -->
      <el-header>
        <header class="header">
          <el-row class="header-left">
            <el-col :span="12"
              ><router-link :to="{ name: 'home' }"
                >鸿宇技术博客</router-link
              ></el-col
            >
            <el-col :span="3"
              ><router-link :to="{ name: 'home' }">首页</router-link></el-col
            >
            <el-col :span="3"><router-link to="/">地图</router-link></el-col>
            <el-col :span="3"><router-link to="/">关于</router-link></el-col>
            <el-col :span="3"><router-link to="/">留言</router-link></el-col>
          </el-row>
          <el-row class="header-right">
            <el-col :span="18">
              <input
                class="search-inp"
                type="text"
                placeholder="输入关键词查找"
              />
            </el-col>
            <el-col :span="6">
              <button class="search-btn">搜索</button>
            </el-col>
          </el-row>
        </header>
      </el-header>

      <!-- 主题内容区 -->
      <el-main>
        <main class="main">
          <div class="main-left">
            <!-- 每日一句 -->
            <div class="every-day">
              <p class="every-day-title">每日一句</p>
              <p class="every-day-content">漫天的星辰是我对你的思念</p>
              <p class="every-day-author">————曹鸿宇</p>
            </div>
            <!-- 博客标题 -->
            <div class="article">
              <p class="article-title">博客标题</p>
              <p class="article-content">
                wn-textarea">飒飒是西安西安西安安心安心安心安属性啊下，，a飒飒是西安西安西安安心安心安心安属性啊下，，a飒飒是西安西安西安安心安心安心安属性啊下，，a飒飒是西安西安西安安心安心安心安属性啊下，，a飒飒是西安西安西安安心安心安心安属性啊下，，a飒飒是西安西安西安安心安心安心安属性啊下
              </p>
              <div class="article-info">
                发布于2020-05-24 | 浏览(6) | Tags：test
              </div>
            </div>

            <div class="article">
              <p class="article-title">博客标题</p>
              <p class="article-content">
                wn-textarea">飒飒是西安西安西安安心安心安心安属性啊下，，a飒飒是西安西安西安安心安心安心安属性啊下，，a飒飒是西安西安西安安心安心安心安属性啊下，，a飒飒是西安西安西安安心安心安心安属性啊下，，a飒飒是西安西安西安安心安心安心安属性啊下，，a飒飒是西安西安西安安心安心安心安属性啊下
              </p>
              <div class="article-info">
                发布于2020-05-24 | 浏览(6) | Tags：test
              </div>
            </div>

            <div class="article">
              <p class="article-title">博客标题</p>
              <p class="article-content">
                wn-textarea">飒飒是西安西安西安安心安心安心安属性啊下，，a飒飒是西安西安西安安心安心安心安属性啊下，，a飒飒是西安西安西安安心安心安心安属性啊下，，a飒飒是西安西安西安安心安心安心安属性啊下，，a飒飒是西安西安西安安心安心安心安属性啊下，，a飒飒是西安西安西安安心安心安心安属性啊下
              </p>
              <div class="article-info">
                发布于2020-05-24 | 浏览(6) | Tags：test
              </div>
            </div>

            <div class="article">
              <p class="article-title">博客标题</p>
              <p class="article-content">
                wn-textarea">飒飒是西安西安西安安心安心安心安属性啊下，，a飒飒是西安西安西安安心安心安心安属性啊下，，a飒飒是西安西安西安安心安心安心安属性啊下，，a飒飒是西安西安西安安心安心安心安属性啊下，，a飒飒是西安西安西安安心安心安心安属性啊下，，a飒飒是西安西安西安安心安心安心安属性啊下
              </p>
              <div class="article-info">
                发布于2020-05-24 | 浏览(6) | Tags：test
              </div>
            </div>

            <!-- 分页插件 -->
            <el-pagination
              background
              class="pagination"
              layout="prev, pager, next"
              @current-change="handleClick"
              :total="1000"
            >
            </el-pagination>
          </div>

          <div class="main-right">
            <div class="tags-cloud">
              <p class="tags-title">随机标签云</p>
              <div class="tags-content">
                <router-link :to="{ name: 'home' }">test</router-link>
                <router-link :to="{ name: 'home' }">zxf</router-link>
                <router-link :to="{ name: 'home' }">chy</router-link>
                <router-link :to="{ name: 'home' }">php</router-link>
                <router-link :to="{ name: 'home' }">node</router-link>
                <router-link :to="{ name: 'home' }">test</router-link>
                <router-link :to="{ name: 'home' }">zxf</router-link>
                <router-link :to="{ name: 'home' }">chy</router-link>
                <router-link :to="{ name: 'home' }">php</router-link>
                <router-link :to="{ name: 'home' }">node</router-link>
                <router-link :to="{ name: 'home' }">test</router-link>
                <router-link :to="{ name: 'home' }">zxf</router-link>
                <router-link :to="{ name: 'home' }">chy</router-link>
                <router-link :to="{ name: 'home' }">php</router-link>
                <router-link :to="{ name: 'home' }">node</router-link>
              </div>
            </div>
            <el-card class="box-card">
              <div slot="header" class="clearfix">
                <span>最近热门</span>
              </div>
              <div v-for="o in 4" :key="o" class="text item">
                {{ "列表内容 " + o }}
              </div>
            </el-card>

            <el-card class="box-card">
              <div slot="header" class="clearfix">
                <span>最新评论</span>
              </div>
              <div v-for="o in 4" :key="o" class="text item">
                <div class="comments"><p>{{ "列表内容 "}}</p> <p>2020-11-02</p></div>
              </div>
            </el-card>
          </div>
        </main>
      </el-main>
      <el-footer class="footer">
          <p class="skills">技术：JavaScript HTML CSS jQuery WebPack Vue React Node MySql 微信小程序 Java</p>
          <p>Copyright @ 2010-2017 啥啥开始讲阿里萨</p>
      </el-footer>
    </el-container>
  </div>
</template>

<script>
export default {
  methods: {
    handleClick(num) {
      console.log(num);
    },
  },
};
</script>

<style lang="scss" scoped>
.el-header {
  background-color: #000;
  color: #333;
  text-align: center;
  height: 60px;
}

.el-footer{
    background-color: #000;
    text-align: center;
    line-height: 30px;
    color:#fff;
    height: 100px !important;
    .skills{
        margin-top: 25px;
    }
}

.header {
  width: 1200px;
  height: 60px;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
  .header-left {
    width: 400px;
    line-height: 60px;
    a {
      color: #fff;
      text-decoration: none;
    }
  }

  .header-right {
    width: 300px;
    line-height: 60px;
    .search-inp {
      width: 220px;
      height: 24px;
      padding: 5px 5px;
      font-size: 14px;
      outline: none;
      border: none;
      border-radius: 5px;
    }
    .search-btn {
      width: 60px;
      height: 35px;
      padding: 5px 5px;
      border-radius: 5px;
      border: none;
      outline: none;
      cursor: pointer;
    }
  }
}

.main {
  width: 1200px;
  margin: 20px auto;
  display: flex;
  justify-content: space-between;
  .main-left {
    width: 750px;
    .every-day {
      width: 100%;
      height: 80px;
      background-color: #ffff;
      border-radius: 10px;
      box-shadow: 0 5px 5px rgba(0, 0, 0, 0.5);
      padding: 10px;
      margin-bottom: 30px;
      box-sizing: border-box;
      .every-day-title {
        text-align: left;
        font-size: 13px;
        color: purple;
      }
      .every-day-content {
        text-align: left;
        font-size: 15px;
        font-weight: 700;
        margin: 10px 0;
      }
      .every-day-author {
        text-align: right;
      }
    }
    .article {
      margin-top: 20px;
      width: 100%;
      height: 140px;
      box-shadow: 0 5px 5px rgba(0, 0, 0, 0.5);
      overflow: hidden;
      background-color: #fff;
      border-radius: 10px;
      text-align: left;
      .article-title {
        font-size: 20px;
        font-weight: 700;
        margin-bottom: 10px;
        padding: 10px 10px 0;
        box-sizing: border-box;
      }
      .article-content {
        width: 100%;
        height: 60px;
        text-indent: 2em;
        font-size: 15px;
        line-height: 20px;
        overflow: hidden;
        margin-bottom: 10px;
        padding: 0 10px;
        box-sizing: border-box;
      }
      .article-info {
        background-color: #000;
        color: #fff;
        width: 100%;
        height: 30px;
        line-height: 30px;
        font-size: 14px;
        padding: 0 15px;
        box-sizing: border-box;
      }
    }
    .pagination {
      margin-top: 20px;
    }
  }

  .main-right {
    width: 400px;
    .tags-cloud {
      width: 100%;
      min-height: 80px;
      background-color: #000;
      padding: 10px 18px;
      border-radius: 15px;
      text-align: left;
      .tags-title {
        color: #fff;
        font-size: 16px;
        margin-bottom: 15px;
      }
      .tags-content {
        width: 100%;
        word-wrap: break-word;
        a {
          text-decoration: none;
          margin: 5px;
        }
      }
    }
    .text {
      font-size: 14px;
    }

    .item {
      margin-bottom: 18px;
    }

    .clearfix:before,
    .clearfix:after {
      display: table;
      content: "";
    }
    .clearfix:after {
      clear: both;
    }

    .box-card {
      width: 100%;
      margin-top: 20px;
      border-radius: 15px;
      background-color: #000;
      color: #fff;
      text-align: left;
      .el-card__header {
        padding: 10px;
        font-size: 15px;
        color: dodgerblue;
      }
    }
    .comments{
        width: 100%;
        display: flex;
        justify-content: space-between;
    }
  }
}
</style>