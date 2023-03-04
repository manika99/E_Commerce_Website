<template>
    <div>
     <footer>
        <p>
            {{ copyright }}
            <a href="https://github.com/manika99">{{github}}</a>
        </p>
     </footer>
    </div>
    </template>
    
    <script>
    export default {
      data () {
        return {
        copyright: 'Copyright || Manika ||',
        github: 'https://github.com/manika99'
        }
      }
    }
    </script>
    
    <style scoped>
    footer{
        background: #222;
        padding: 6px;
    }
    p{
        color: lightgreen;
        text-align: center;
    }
    a{
      color: lightgreen;
      text-decoration: none;
    }
    
    </style>