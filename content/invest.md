+++
+++


{{< rawhtml >}} 
<span id="logt">Please enter Investor Code below to see video:</span>
<input id="invest" type="text" placeholder="Investor Code" >
<video
    id="invid"
    style="margin: 0 auto; display:none"
    width=70%
    controls
    
    poster=/img/cover.png>
    <source src="/videos/explainer480.mp4" type="video/mp4">
    Your browser does not support the video tag.  
</video>
<script>
{
let invest = document.getElementById('invest')
let invid = document.getElementById('invid')
let logt = document.getElementById('logt')


function dumbLogin () {
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
