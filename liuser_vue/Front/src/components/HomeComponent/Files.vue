<template>
  <div
  id="#filedownload"
    class="file-dowload"
    style="position:relative; height:500px; overflow:hidden"
  >
  <h1>{{ files.title }}</h1>
    <div v-for="item in files.fileArr" :key="item" >
          <span style="font-size:15px">{{item.name}}</span>
          <a :href="item.downloadUrl" target="_blank">
            <i class="fa fa-arrow-circle-down" ></i>
          </a>
            
        </div>
  </div>
</template>

<script>
export default {
  data(){
    return{
      files:{
        title:'比赛的通知文件',
        fileArr:[
          {
          name:"2018年比赛的通知文件",
          downloadUrl:'https://user-gold-cdn.xitu.io/2020/3/29/17125992d200dfe3?w=980&h=320&f=jpeg&s=82086'
        },
          {
          name:"2017年比赛的通知文件",
          downloadUrl:'https://user-gold-cdn.xitu.io/2020/3/29/17125992d200dfe3?w=980&h=320&f=jpeg&s=82086'
        },
          {
          name:"2016年比赛的通知文件",
          downloadUrl:'https://user-gold-cdn.xitu.io/2020/3/29/17125992d200dfe3?w=980&h=320&f=jpeg&s=82086'
        },
          {
          name:"2015年比赛的通知文件",
          downloadUrl:'https://user-gold-cdn.xitu.io/2020/3/29/17125992d200dfe3?w=980&h=320&f=jpeg&s=82086'
        },
        ]
        }
    }
  }
};
</script>

<style scoped>
h1{
  font-size:2rem;
}
.file-dowload{
  display:flex;
  flex-direction: column;
}
.fa{
  cursor: pointer;
  color: #FF7043;
}
a{
  margin-left:10px;
  font-size: 17px;
  
}
</style>
