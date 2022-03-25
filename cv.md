# Evghen Sykalov CV

### Contact information
* 067-595-1927
* Ukraine, Kyiv
* evgeniy2chainzdev@gmail.com
* tg: evg2chainz

### Personal profile
* Learn quick
* A desire to develop and grow 
* Ability to solve difficult assignment
* Perfectionistic and diplomatic
* Team-building
* Absence of bad habits
* Self-team development

### Experience
* Operating systems: Unix, Windows, iOs, Android 
* Languages: JavaScript, Node Js, React, HTML, CSS
* Database: MongoDb
* A lot of other tools: MsOficce, VirtualBox / VMWare / Nox, Antidectes, Photoshop, Cubase

### Education 
* Inoxoft NodeJs Intern
* JavaScript, React (Way of samurai)
* NTUU KPI / Faculty of electronics, master’s degree / 2006-2011
* Technical Lyceum NTUU KPI / class with advanced study physic and mathematic / 2000-2006

### Career history
#### Freelance / 2015 - nowadays
_Responsibilities_
* Affiliate marketing
* Antifraud systems
* Beta testing
* Multi-accounting
_OS, Tools, languages_
Keitaro, Landings, VPS, Antidectes, VirtualBox / VMWare / Nox
#### VTB Bank / IT Systems Analyst / 2011 - 2015
_Responsibilities_
* Working with bug tracking tool
* Product, server support
* Product release
* Communication with developers, product managers, call-center
_OS, Tools, languages_
Releasing, Bug tracking tool, iFobs, iFobs web version, B2, Oracle SQL, Unix

### Code example
```
// accordeon-start

let footerColumn  = document.getElementsByClassName("footer-column-ul");

// console.log(footerColumn);

for (let i = 0; i < footerColumn.length-1; i++) {
    footerColumn[i].onclick = function () {
        if (footerColumn[i].classList.contains('accordeon-footer-active')) {
            // console.log('condition1_ActiveAccordeonClassHere') ;
            let arrowVarD2R = document.querySelector('.accordeon-footer-active .footer-column__title__arrow')
            arrowVarD2R.src='img/svg/arrow-right.svg';
            footerColumn[i].classList.remove("accordeon-footer-active")
            let x = footerColumn[i].querySelector('.footer-column__title');
            console.log('click'+x)
            x.classList.add("footer-column__title_underlined")
            // console.log(arrowVarD2R) ;

        } else {
            // console.log('condition2_noActiveAccordeonClassHere') ;
            for (let j = 0; j < footerColumn.length - 1; j++) {
                footerColumn[j].classList.remove("accordeon-footer-active");

                // console.log('removing all active classes ')
            }
            //to all titles add underlines start
            let y = document.querySelectorAll('.footer-column__title');
            console.log(y);
            for (let g=0; g<y.length-1;g++){
                y[g].classList.add('footer-column__title_underlined');
            }
            //to all titles add underlines end

            // console.log(document.getElementsByClassName('footer-column__title__arrow'))
            let arrOfAllArrows = document.getElementsByClassName('footer-column__title__arrow')
            // console.log('arrOfAllArrows = ' + arrOfAllArrows);
            //all arrows to right
            for (let z = 0; z < arrOfAllArrows.length-1; z++) {
                arrOfAllArrows[z].src='img/svg/arrow-right.svg'
            }

            footerColumn[i].classList.add("accordeon-footer-active");
            let arrowVarR2D = document.querySelector('.accordeon-footer-active .footer-column__title__arrow')
            // console.log(arrowVarR2D) ;
            arrowVarR2D.src='img/svg/arrow-bottom.svg';
            let z = footerColumn[i].querySelector('.footer-column__title_underlined');
            console.log('click'+z)
            z.classList.remove("footer-column__title_underlined")
            // console.log($(footerColumn[i]).children('h3'))
            // footerColumn[i].classList.toggle('footer-column__title_underlined');


        }
    }
}
// accordeon-end
```