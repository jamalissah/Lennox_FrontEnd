<template>
    <footer class="footer">
    <div class="leftside">
                <p>&copy; 2024</p>
            </div>
            <div class="rightside">        
                <a href="#"><img src="https://th.bing.com/th/id/R.2bad70f2d08429a28dfbebd4c237924b?rik=vgEdhJ%2f%2biiEnQQ&riu=http%3a%2f%2fpngimg.com%2fuploads%2ffacebook_logos%2ffacebook_logos_PNG19748.png&ehk=0ZiZ04ZZ6mSJ5oyPxBh1gy4FSYhegWTWyDpCiI73sbw%3d&risl=&pid=ImgRaw&r=0" alt=""></a>
                <a href="#"><img src="https://th.bing.com/th/id/OIP.JtmXSh_uyZBaTg1eXd-NtgHaHa?rs=1&pid=ImgDetMain" alt=""></a>
                <a href="#"><img src="https://th.bing.com/th/id/R.c3fcc390427d68b89647e834adf7fc87?rik=5W%2fa9g9fys8WDg&pid=ImgRaw&r=0" alt=""></a>
            </div>
    </footer> 
</template>

<script>
export default{
    name: 'MyFooter'
};
</script>

<style scoped>

  .footer {
  background-color: #333;
  color: white;
  text-align: center;
  margin: 50px 0px 0px 0px;
  position: relative;
  bottom: 0;
  width: 100%;
  height: 50px; 
  }

  footer .leftside{
            float: left;
            display: flex;
        }
        
        footer .leftside img{
            max-width: 50px;
            padding: 5px;
            margin-bottom: 0px;
            padding-bottom: 0px;
        }
        
        footer .rightside{
            float: right;
        }
        
        footer a {
            float: left;
            display: block;
            color: #f2f2f2;
            text-align: center;
            font-size: 17px;
        }
        
        footer a:hover{
            color: black;
        }
        
        .rightside{
            padding: 5px;
        }
        
        .rightside img {
            border-radius: 50%;
            margin: 10px;
            margin-bottom:0px;
            max-width: 30px;
            transition: transform 0.2s ease;
            margin-bottom: 0px;
            padding-bottom: 0px;
        }
          
        .rightside img:hover {
            transform: scale(1.5);
        }
  </style>