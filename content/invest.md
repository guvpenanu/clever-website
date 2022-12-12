+++
+++


{{< rawhtml >}} 
<span id="logt">Please enter Investor Code below to see video:</span>
<input id="invest" type="text" placeholder="Investor Code" >

<div id="invid" style="margin: 0 auto; display:none">


<video
    
    style="margin: 0 auto;"
    width=90%
    controls
    
    poster=/img/cover.png>
    <source src="/videos/explainer480.mp4" type="video/mp4">
    Your browser does not support the video tag.  
</video>

<style>
.clever {
    color: blue;
}
.copyw {
    width: 90%;
    margin: 0 auto;
}

.blurb {
    display: flex;
}

.blurb div {
flex: 10;
text-align: justify;
text-justify: inter-word;
}
.blurb div.divider {
flex: 1;

}

a {
color: blue;
text-decoration: underline;
}

</style>

<br/>

<div class="copyw">

    <div class="blurb">
        <div>
            <span class="clever">clever</span> makes complex decisions simple and analyzable through the carbon credit project cycle.  Read how all stakeholders benefit from clever’s proprietary smart database <a target="_blank" href="/pdf/complex-to-simple.pdf#toolbar=0&navpanes=0">here</a>.
        </div>
        <div class="divider"></div>
        <div>
            <span class="clever">clever's</span> proprietary database is the largest of its kind, aggregating project details for carbon markets.  Read about our special sauce <a target="_blank" href="/pdf/special-sauce.pdf#toolbar=0&navpanes=0">here</a>.
        </div>
    </div>


</div>


<br/>




<video
    
    style="margin: 0 auto;"
    width=90%
    controls
    
    poster=/img/simple.png>
    <source src="/videos/complicated.mp4" type="video/mp4">
    Your browser does not support the video tag.  
</video>

</div>

<script>
{
console.log('run that ')
let invest = document.getElementById('invest')
let invid = document.getElementById('invid')
let logt = document.getElementById('logt')


function dumbLogin () {
    console.log(invest.value.trim().toLowerCase())
    if (invest.value.trim().toLowerCase() == 'invest' || localStorage.getItem('login') ) {
        invid.style.display = 'block'
        invest.style.display = 'none'
        logt.style.display = 'none'
        localStorage.setItem('login', true)
    }
        
    
} 

invest.onkeyup = dumbLogin
dumbLogin()

}
</script> 
{{< /rawhtml >}}
