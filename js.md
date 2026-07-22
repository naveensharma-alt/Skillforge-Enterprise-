
// ============================
// MOBILE MENU
// ============================


const menuBtn = document.querySelector(".menu");
const nav = document.querySelector("nav");


menuBtn.addEventListener("click", () => {

    nav.classList.toggle("active");

});





// ============================
// COUNTER ANIMATION
// ============================


const counters = document.querySelectorAll(".counter");


const startCounter = (counter)=>{


    const target = +counter.dataset.target;

    let count = 0;

    const speed = target / 100;


    const update = ()=>{


        if(count < target){

            count += speed;

            counter.innerText = Math.ceil(count);

            setTimeout(update,20);

        }

        else{

            counter.innerText = target;

        }


    };


    update();


};





const observer = new IntersectionObserver((entries)=>{


entries.forEach(entry=>{


    if(entry.isIntersecting){

        startCounter(entry.target);

        observer.unobserve(entry.target);

    }


});


},
{
    threshold:.5
});



counters.forEach(counter=>{

    observer.observe(counter);

});







// ============================
// FAQ ACCORDION
// ============================


const faqButtons = document.querySelectorAll(".faq-item button");


faqButtons.forEach(button=>{


    button.addEventListener("click",()=>{


        const parent = button.parentElement;


        document.querySelectorAll(".faq-item")
        .forEach(item=>{

            if(item !== parent){

                item.classList.remove("active");

            }

        });



        parent.classList.toggle("active");


    });


});






// ============================
// TESTIMONIAL SLIDER
// ============================



const testimonials=[

{

text:
"SkillForge helped us create a strong learning culture and improved employee productivity.",

author:
"- HR Director, Technology Company"

},


{

text:
"The customized enterprise programs matched our business goals perfectly.",

author:
"- Learning Manager, Global Organization"

},


{

text:
"Analytics and reporting helped us measure real training impact.",

author:
"- Operations Head, Enterprise Firm"

}

];



let currentTestimonial=0;



const quote=document.getElementById("quote");

const author=document.getElementById("author");



function changeTestimonial(){


currentTestimonial++;


if(currentTestimonial >= testimonials.length){

    currentTestimonial=0;

}



quote.style.opacity=0;

author.style.opacity=0;



setTimeout(()=>{


quote.innerText=testimonials[currentTestimonial].text;

author.innerText=testimonials[currentTestimonial].author;


quote.style.opacity=1;

author.style.opacity=1;


},300);


}



setInterval(changeTestimonial,4000);







// ============================
// SMOOTH SCROLL
// ============================


document.querySelectorAll("a[href^='#']")
.forEach(anchor=>{


anchor.addEventListener("click",function(e){


const target=document.querySelector(
this.getAttribute("href")
);


if(target){

e.preventDefault();


target.scrollIntoView({

behavior:"smooth"

});


}


});


});







// ============================
// CONTACT FORM VALIDATION
// ============================


const form=document.querySelector("form");


form.addEventListener("submit",(e)=>{


e.preventDefault();


const inputs=form.querySelectorAll("input, textarea");


let valid=true;



inputs.forEach(input=>{


if(input.value.trim()===""){


valid=false;

input.style.border="1px solid red";


}

else{


input.style.border="1px solid #d0d5dd";


}


});



if(valid){


alert(
"Thank you! Our team will contact you soon."
);


form.reset();


}


});







// ============================
// SCROLL REVEAL EFFECT
// ============================


const revealElements=document.querySelectorAll(
".card,.program,.stat-box,.about-box"
);



const revealObserver=new IntersectionObserver(
(entries)=>{


entries.forEach(entry=>{


if(entry.isIntersecting){


entry.target.style.opacity="1";

entry.target.style.transform="translateY(0)";


}


});


},
{
threshold:.2
});



revealElements.forEach(element=>{


element.style.opacity="0";

element.style.transform="translateY(40px)";

element.style.transition=
"all .6s ease";


revealObserver.observe(element);


});
