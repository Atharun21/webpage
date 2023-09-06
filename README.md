burger = document.querySelector('.burger')
navbar=document.querySelector('.navbar')
rightNav = document.querySelector('.rightNav')
navList=document.querySelector('.nav-list')


burger.addEventListener('click', ()=>{
    rightNav.classList.toggle('v-class-resp');
    nav-list.classList.toggle('v-class-resp');
    navbar.classList.toggle('h-nav-resp');

})
 254 changes: 254 additions & 0 deletions254  
webpage/css/style.css
@@ -0,0 +1,254 @@
@import url('https://fonts.googleapis.com/css2?family=Ubuntu:ital,wght@1,500&display=swap');
*{
    margin:0;
    padding:0;
}

html{
    scroll-behavior: smooth;
}

.logo{
    width: 20%;
    display: fiex;
    justify-content: center;
    align-items: center;
}
.logo img{
    width: 26%;
    border: 3px solid white;
    border-radius: 50px;
    margin: 5px;
}
.navbar{
    display: flex;
    align-items: center;
    justify-content: center;
    position: sticky;
    top: 0;
    cursor: pointer;


}

.nav-list{
    width:70%;
    display: flex;
    align-items: center;

}

.nav-list li{
    list-style: none;
    padding: 26px 30px;

}

.nav-list li a{
    text-decoration: none;
    color: black;
    font-size: 20px;
    font-family: 'ubuntu',sans-serif;


}
.nav-list li a:hover{
    color: gray;


}
.rightNav{
    width:30%;
    text-align: right;
    padding: 0 23px;
}
#search{
    padding: 5px;
    font-size: 17px;
    border: 2px solid gray;
    border-radius: 9px;
}
.background{
    background: rgba(0, 0, 0, 0)url(../img/bg.jpg);
    background-size: cover;
    background-blend-mode: darken;
}

.firstsection{
    height: 100vh;
}
.box-main{
    display: flex;
    justify-content: center;
    align-items: center;
    color: black;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    max-width: 50%;
    margin: auto;
}

.firstHalf{
    width: 80%;
    display: flex;
    flex-direction: column;
    justify-content: center;

}
.secondHalf{
    width: 30%;
}
.secondHalf img{
    width: 70%;
    padding: 1px;
    border: 4px solid white;
    border-radius: 160px;
    display: block;
    margin: auto;
}
.text-big{
    font-size: 41px;
    padding-left: 20px;
}
.text-small{
    font-size: 18px;
    padding-left: 20px;
}
.btn{
    padding: 8px 20px;
    margin: 7px 3px;
    border: 2px solid white;
    border-radius: 8px;
    background: none;
    color: white;
    cursor: pointer;
    font-family: 'ubuntu',sans-serif;
    font-size: 20px;
}
.btn-sm{
    padding: 6px 10px;
    vertical-align: middle;
    font-size: 16px;
}
.btn-dark{
    color: black;
    border: 2px solid gray;
}
.section{
    display: flex;
    align-items: center;
    justify-content: space-evenly;
    max-width: 80%;
    margin: auto;
    font-family:'ubuntu',sans-serif;
    padding: 10px;
}
.section-Left{
    flex-direction: row-reverse;
    padding-right: 10px;
}
.sectionTag{
    padding: 16px 0;
}
.sectionSubTag{
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}
.thumbnail{
    height: 250px;
    width: 250px;
    border: 4px solid black;
    border-radius: 10px;
    margin-top: 19px;
}
.contact{
    background-color: #f6f5f4;
    height: 150vh;
}
.text-center{
    text-align: center;
    padding: 30px;
    font-family:'ubuntu',sans-serif;
    font-size: 40px;
}
.form{
    max-width: 62%px;
    margin:  42px auto;
}
.form-input{
    margin: 30px 0;
    padding: 5px 3px;
    width: 100%;
    font-size: 19px;
    border: 2px solid grey;
    border-radius: 6px;
}
.text-footer{
    padding: 30px 0px;
    text-align: center;
    font-family:'ubuntu',sans-serif;
    display: flex;
    justify-content: center;

}


.burger{
    display: none;
    position: absolute;
    cursor: pointer;
    right: 5%;
    top: 15px;

}
.line{
    width: 33px;
    background-color: white;
    height: 4px;
    margin: 3px 3px; 
}

@media screen and (max-width:1140px) {
    .nav-list{
        flex-direction: column;
    }
    .navbar{
        height: 447px;
        flex-direction: column;
        transition: all 0.3 ease-out;
    }
    .rightNav{
        text-align: center;
    }
    .box-main{
        flex-direction: column-reverse;
        max-width: 100%;
    }
    #search{
        width: 100%;
    }
    .burger{
        display: block;
    }
    .h-nav-resp{
        height: 150px;
    }
    .v-class-resp{
        opacity: 0;
    }
    .section{
        flex-direction: column-reverse;

    }
    .text-small{
        text-align: center;
    }
    .text-big{
        text-align: center;
    }
    .buttons{
        text-align: center;
    }
    .paras{
        padding: 0px ;
    }

}
 Binary file addedBIN +32.3 KB 
webpage/img/bg.jpg

 Binary file addedBIN +11.6 KB 
webpage/img/img.jpg

 178 changes: 178 additions & 0 deletions178  
webpage/index.html
@@ -0,0 +1,178 @@
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="css/style.css">
    <link rel="stylesheet" href="css/responsive.css" class="rel">

    <title>The Internet of Things
    </title>
</head>

<body>
    <nav class="navbar background h-nav-resp">
        <ul class="nav-list v-class-resp">
            <div class="logo"><img src="img/img.jpg" alt="logo"></div>
            <li><a href="#home">home</a></li>
            <li><a href="#about">about</a></li>
            <li><a href="#services">services</a></li>
            <li><a href="#contact us">contact us</a></li>
        </ul>
        <div class="rightNav v-class-resp">
            <input type="text" name="search" id="search">
            <button class="btn btn-sm">search</button>
        </div>
        <div class="burger">
            <div class="line"></div>
            <div class="line"></div>
            <div class="line"></div>
        </div>
    </nav>
    <section class="background firstsection">
        <div class="box-main">
            <div class="firstHalf">
                <p class="text-big"> “The Internet of Things is going to be a real gamechanger for loyalty, just like mobile has been to date.”.</p>
                <p class="text-small">“If you think that the internet has changed your life, think again. The Internet of Things is about to change it all over again!”</p>
                <div class="button">
                    <button class=" btn">subscribe</button>
                    <button class="btn">watch video</button>
                </div>
            </div>

            <div class="secondHalf">
                <img src="img/img.jpg" alt="laptop image">
            </div>
        </div>

    </section>
    <section class="section">
        <div class="paras">
            <p class="sectionTag text-big">  Internet of Things
            </p>
            <p class="sectionSubTag text-small">
                The Internet of Things (IoT) is the ability to have devices communicate with one another via the internet or other
                 networks, remotely tracking information to provide feedback to assist with decision making for commercial, industrial
                  and residential purposes. This is commonly done using sensors connecting to a back-to-base system.

                Some common day-to-day examples could be:

                Temperatures in refrigeration or food heating units in the food and beverage industry.
                Assistance with the control of temperature and humidity levels.
                Detection of gas and dust levels.
                Monitoring of water levels and herd locations for agricultural purposes.
                Different applications in the automotive, aviation and nautical sectors such as the sensing of 
                tyre pressures for trucking fleets.
                </p>
        </div>
        <div class="thumbnail">
            <img src="https://source.unsplash.com/250x250/?coding,apple" alt="loptop image" class="imgFluid">
        </div>
    </section>
    <section class="section section-Left" id="about">
        <div class="paras">
            <p class="sectionTag text-big">What History of IOT?</p>
            <p class="sectionSubTag text-small">
                The main concept of a network of smart devices was discussed as early as 1982, with a modified Coca-Cola vending machine at 
                 Carnegie Mellon University becoming the first ARPANET-connected appliance,[13] able to report its inventory and whether newly
                  loaded drinks were cold or not.[14] Mark Weiser's 1991 paper on ubiquitous computing, "The Computer of the 21st Century", as 
                  well as academic venues such as UbiComp and PerCom produced the contemporary vision of the IOT. In 1994, Reza Raji 
                  described the concept in IEEE Spectrum as "[moving] small packets of data to a large set of nodes, so as to integrate and 
                  automate everything from home appliances to entire factories". Between 1993 and 1997, several companies proposed solutions
                   like Microsoft's at Work or Novell's NEST. The field gained momentum when Bill Joy envisioned device-to-device communication
                    as a part of his "Six Webs" framework, presented at the World Economic Forum at Davos in 1999.


                The concept of the "Internet of things" and the term itself, first appeared in a speech by Peter T. Lewis, to the Congressional 
                Black Caucus Foundation 15th Annual Legislative Weekend in Washington, D.C., published in September 1985. According to Lewis, 
                "The Internet of Things, or IoT, is the integration of people, processes and technology with connectable devices and sensors to 
                enable remote monitoring, status, manipulation and evaluation of trends of such devices.

                The term "Internet of things" was coined independently by Kevin Ashton of Procter & Gamble, later of MIT's Auto-ID Center, in
                 1999,[21] though he prefers the phrase "Internet for things".[22] At that point, he viewed radio-frequency identification 
                 (RFID) as essential to the Internet of things,[23] which would allow computers to manage all individual things.
                  The main theme of the Internet of things is to embed short-range mobile transceivers in various gadgets and daily necessities 
                  to enable new forms of communication between people and things, and between things themselves.

                In 2004 Cornelius "Pete" Peterson, CEO of NetSilicon, predicted that, "The next era of information technology will be
                 dominated by [IoT] devices, and networked devices will ultimately gain in popularity and significance to the extent 
                 that they will far exceed the number of networked computers and workstations." Peterson believed that medical devices 
                 and industrial controls would become dominant applications of the technology.

                Defining the Internet of things as "simply the point in time when more 'things or objects' were connected to the Internet
                 than people", Cisco Systems estimated that the IoT was "born" between 2008 and 2009, with the things/people ratio growing 
                 from 0.08 in 2003 to 1.84 in 2010.
        <div class="thumbnail">
            <img src="https://source.unsplash.com/250x250/?coding,apple,html" alt="loptop image" class="imgFluid">
        </div>
    </section>
    <section class="section" id="services">
        <div class="paras">
            <p class="sectionTag text-big">Social Internet of things?</p>
            <p class="sectionSubTag text-small">
                Social Internet of things (SIoT) is a new kind of IoT that focuses the importance of social
                 interaction and relationship between IoT devices. SIoT is a pattern of how cross-domain
                  IoT devices enabling application to application communication and collaboration without human
                   intervention in order to serve their owners with autonomous services,[156] and this only can be
                   realized when gained low-level architecture support from both IoT software and hardware engineering.[157]
                Social Network for IoT Devices (Not Human)
                IoT defines a device with an identity like a citizen in a community and connect them to the internet 
                to provide services to its users.[158] SIoT defines a social network for IoT devices only to interact
                 with each other for different goals that to serve human.

                How is SIoT different from IoT?
                SIoT is different from the original IoT in terms of the collaboration characteristics. IoT is passive,
                 it was set to serve for dedicated purposes with existing IoT devices in predetermined system. SIoT is
                  active, it was programmed and managed by AI to serve for unplanned purposes with mix and match of potential 
                  IoT devices from different systems that benefit its users.

                How does SIoT Work?
                IoT devices built-in with sociability will broadcast their abilities or functionalities, and at the same time
                 discovers, navigates and groups with other IoT devices in the same or nearby network for useful service 
                 compositions in order to help its users proactively in every day's life especially during emergency.

                Social IoT Examples
                IoT-based smart home technology monitors health data of patients or aging adults by analyzing their physiological
                 parameters and prompt the nearby health facilities when emergency medical services needed. In case emergency,
                  automatically, ambulance of a nearest available hospital will be called with pickup location provided, ward assigned,
                   patient's health data will be transmitted to the emergency department, and display on the doctor's computer immediately
                    for further action.
                IoT sensors on the vehicles, road and traffic lights monitor the conditions of the vehicles and drivers and alert when
                attention needed and also coordinate themselves automatically to ensure autonomous driving is working normally. 
                Unfortunately if an accident happens, IoT camera will inform the nearest hospital and police station for help.[164]
                Social IoT Challenges
                Internet of things is multifaceted and complicated.One of the main factors that hindering people
                 from adopting and use Internet of things (IoT) based products and services is its complexity.[166] Installation
                  and setup is a challenge to people, therefore, there is a need for IoT devices to mix match and configure 
                  themselves automatically to provide different services at different situation.
                System security always a concern for any technology, and it is more crucial for SIoT as not only security 
                of oneself need to be considered but also the mutual trust mechanism between collaborative IoT devices from
                 time to time, from place to place.
                Another critical challenge for SIoT is the accuracy and reliability of the sensors. At most of the circumstances,
                 IoT sensors would need to respond in nanoseconds to avoid accidents, injury, and loss of life.
            </p>
        </div>
        <div class="thumbnail">
            <img src="https://source.unsplash.com/250x250/?javascript,apple" alt="loptop image" class="imgFluid">
        </div>
    </section>
    <section class="Contact" id="Contact">
        <h2 class="text-center">ContactUs</h2>
        <div class="form">
            <input class="form-input" type="text" name="name" id="name" placeholder="Enter Your Name">
            <input class="form-input" type="text" name="phonenumber" id="phonenumber"
                placeholder="Enter Your phonenumber">
            <input class="form-input" type="text" email="email" id="email" placeholder="Enter Your email">
            <textarea class="form-input" name="text" id="" cols="30" rows="10" class="text"
                placeholder="how was ur experience"></textarea>
            <button class="btn btn-dark">Submit</button>
    </section>
    <footer class="background">
        <p class="text-footer">Copyright &copy; 2027- All right reserved</p>
    </footer>
    <script src="js/resp.js"></script>


</body>

</html>
