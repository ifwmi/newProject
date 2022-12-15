<template>
  <div class="container">
      <div class="list">
        <div class="item" v-for="person in people" :class="`bg-${person.color}`">
          <span class="name">{{ person.name }}</span>
          <span>-</span>
          <span class="type">{{ person.type }}</span>
        </div>
      </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      people: []
    }
  },
  mounted() {
    this.people.push({
      name: 'Danil',
      type: 'mentor',
      color: 'purple'
    }),
    this.people.push({
      name: 'Islam',
      type: 'Student',
      color: 'yellow'
      
    })
    this.people.push({
      name: 'John',
      type: 'mentor',
      color: 'red'
    }),
    this.people.push({
      name:'Iman',
      type:'student',
      color: 'papayawhip'
    })
    this.people.push({
      name: 'Nikita',
      type: 'student',
      color: 'orange'
    }),
    this.people.push({
      name: 'AbuBandit',
      type: 'student',
      color: 'yellow'
    })
    this.people.push({
      name: 'Kalybek',
      type: 'student',
      color: 'you-best'
    })
    this.people.push({
      name: 'Bekjan',
      type: 'student scientist',
      color: 'mediumblue'
    })
    this.people.push({
      name: 'Anton',
      type: 'student',
      color: 'mediumaquamarine'
    })
    
    this.people.push({
      name: 'bekzat',
      type: 'student',
      color: 'palevioletred'
    })
    this.people.push({
      name: 'Ken',
      type: 'student',
      color: 'black'
    })
    this.people.push({
      name: 'Mansur',
      type: 'student',
      color: 'blue'
    })
    //здесь будете пушить свои данные
  }
}
</script>

<style>
  .list {
    display: flex;
    flex-wrap: wrap;
  }
  .list .item {
    width: 50%;
    display: flex;
    color: white;
    font-size: 22px;
    padding: 30px 10px;
    justify-content: center;
    font-weight: 500;
  }
  .list .item .name {
    margin-right: 10px;
  }
  .list .item .type {
    margin-left: 10px;
  }
  .list .bg-purple {
    background: #810281;
  }
  .list .bg-yellow {
    background: #ffa200;
    font-family:'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
    font-weight: bold;
  }
  
  .list .bg-red {
    background: #fd0d0d;
  }
  .list .bg-papayawhip {
    background: papayawhip;
    color: black;
  } 
  .list .bg-orange {
    background: orange;
  }
  .list .bg-you-best {
    background: rgb(53, 45, 31);
  }
  .list .bg-mediumblue{
    background: mediumblue;
    color: gold;
  }
  .list .bg-mediumaquamarine {
    background: mediumaquamarine;
  }
  .list .bg-black {
    background: #0d69b0;
  }
  .list .bg-blue {
    background: #020c13;
  }
  .list .bg-yellow {
    background: rgb(242, 255, 0);
  }
</style>