# My-first-project
For learning english
*{
   margin: 0;
   padding: 0;
   font-family: 'Big Shoulders Stencil Display', cursive;
}
.header{
    min-height: 100vh;
    width: 100%;
    background-image:linear-gradient(rgba(4,9,30,0.7),rgba(4,9,30,0.7)),url(
        images/pexels-pixabay-2.jpg);
    background-position: center;
    background-size: cover;
    position: relative;

}
nav{
    display: flex;
    padding: 2% 6%;
    justify-content: space-between;
    align-items: center;
    
}
nav img{
    width: 150px;
}

.nav-links{
    flex: 1;
    text-align: right;
}
.nav-links ul li{
    list-style: none;
    display: inline-block;
    padding: 8px 12px;
    position: relative;
}
.nav-links ul li a{
    color:#fff;
    text-decoration: none;
    font-size: 13px;
}
.nav-links ul li::after{
    content: '';
    width: 0%;
    height: 2px;
    background: #f44336;
    display: block;
    margin: auto;
    transition: 0.5s;
}
.nav-links ul li:hover::after{
    width: 100%;
}

.text-box{
    width: 90%;
    color: #fff;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%,-50%);
    text-align: center;
}
.text-box h1{
    font-size: 62px;
}
text-box p{
    margin: 10px 0 40px;
    font-size: 14px;
    color: #fff;
}
.hero-btn{
    display: inline-block;
    text-decoration: none;
    color: #fff;
    border: 1px solid #fff;
    padding: 12px 34px;
    font-size: 13px;
    background: transparent;
    position: relative;
    cursor: pointer;
}
.hero-btn:hover{
    border: 1px solid #f44336;
    background: #f44336;
    transition: 1s;
}

nav .fa{
    display: none;
}

@media(max-width: 700px){
    text-box h1{
        font-size: 62px;
    }
    .nav-links ul li{
        display: block;
    }
    .nav-links{
        position: absolute;
        background: #f44336;
        height: 100vh;
        width: 200px;
        top: 0;
        right: -200px;
        text-align: left;
        z-index: 2;
        transition: 1s;
    }
    nav .fa{
        display: block;
        color: #fff;
        margin: 10px;
        font-size: 22px;
        cursor: pointer;
    }
    .nav-links ul{
        padding: 30px;
    }
}

/*----- course -----*/

.course{
    width: 80%;
    margin: auto;
    text-align: center;
    padding-top: 100px;
}
h1{
    font-size: 36px;
    font-weight: 600;
}

p{
    color: #777;
    font-size: 14px;
    font-weight: 300;
    line-height: 22px;
    padding: 10px;
}

.row{
    margin-top: 5%;
    diplay: flex;
    justify-content: space-between;
}
.course-col{
    flex-basis: 31%;
    background: #fff3f3;
    border-radius: 10px;
    margin-bottom: 5%;
    padding: 20px 12px;
    box-sizing: border-box;
    transition: 0.5s;
}
h3{
    text-align: center;
    font-weight: 600;
    margin: 10px 0;
}
.course-col:hover{
    box-shadow: 0 0 20px 0px rgba(0,0,0,0.2);
}
@media(max-width: 700px){
    .row{
        flex-direction: column;
    }
}

/*----- campus -----*/
.campus{
    width: 80%;
    margin: auto;
    text-align: center;
    padding-top: 50px;
}
.campus-col{
    flex-basis: 32%;
    border-radius: 10px;
    margin-bottom: 30px;
    position: relative;
    overflow: hidden;
}
.campus-col img{
    width: 100%;
    display: block;
}
.layer{
    background: transparent;
    height: 100%;
    width: 100%;
    position: absolute;
    top: 0;
    left: 0;
    transition: 0.5s;
}
.layer:hover{
 background: rgba(226,0,0,0.7);
}

.layer h3{
    width: 100%;
    font-weight: 500;
    color: #fff;
    font-size: 26px;
    bottom: 0;
    left: 50%;
    transform: translateX(-50%);
    position: absolute;
    opacity: 0;
    transition: 0.5s;
}
.layer:hover h3{
    bottom: 49%;
    opacity: 1;
}

/*----- facilities -----*/

.facilities{
    width: 80%;
    margin: auto;
    text-align: center;
    padding-top: 100px;
}

.facilities-col{
    flex-basis: 31%;
    border-radius: 10px;
    margin-bottom: 5%;
    text-align: left;
}

.facilities-col img{
    width: 100%;
    border-radius: 10px;
}

.facilities-col p{
    padding: 0;
}

.facilities-col h3{
    margin-top: 16px;
    margin-bottom: 15px;
    text-align: left;
}

/*----- testimonials -----*/

.testimonial{
    width: 80%;
    margin: auto;
    padding-top: 100px;
    text-align: center;
}

.testimonial-col{
    flex-basis: 44%;
    border-radius: 10px;
    margin-bottom: 5%;
    text-align: left;
    background: #fff3f3;
    padding: 25px;
    cursor: pointer;
    display: flex;
}

.testimonial-col img{
    height: 40px;
    margin-left: 5px;
    margin-right: 30px;
    border-radius: 50%;
}

.testimonial-col p{
    padding: 0;
}

.testimonial-col h3{
    margin-top: 15px;
    text-align: left;
}

.testimonial-col .fa{
    color: #f44336;
}

@media(max-width: 700px){
    
.testimonial-col img{
    margin-left: 0px;
    margin-right: 15px;
  }
}

/* call to action */

.cta{
    margin: 100px auto;
    width: 80%;
    background-image: linear-gradient(rgba(0,0,0,0.7),rgba(0,0,0,0.7)),url(images/banner2.jpg);
    background-position: center;
    background-size: cover;
    border-radius: 10px;
    text-align: center;
    padding: 100px 0;
}

.cta h1{
    color: #fff;
    margin-bottom: 40px;
    padding: 0;
}

@media(max-width: 700px) {
    .cta h1{
        font-size: 24px;
    }
}

/*-----footer-----*/
.footer{
    width: 100%;
    text-align: center;
    padding: 30px 0;
    
.footer h4{
    margin-bottom: 25px;
    margin-top: 20px;
    font-weight: 600;
    }
}
.icons .fa{
    color: #f44336;
    margin: 0 13px;
    cursor: pointer;
    padding: 18px 0;
}
.fa-heart-o{
    color: #f44336;
}

/* ----- About Us page ----- */

.sub-header{
    height: 50vh;
    width: 100%;
    background-image: linear-gradient(rgba(4,9,30,0.7),(rgba(4,9,30,0.7)),url(images/background.jpg);
    background-position: center;
    background-size: cover;
    text-align: center;
    color: #fff;
}

.sub-header h1{
    margin-top: 100px;
}

.about-us{
    width: 80%;
    margin: auto;
    padding-top: 80px;
    padding-bottom: 50px;   
}

.about-col{
    flex-basis: 48p%;
    padding: 30px 2px;
}

.about-col img{
    width: 100%;
}

.about-col h1{
    padding-top: 0;
}
.about-col p{
    padding: 15px 0 25px;
}
