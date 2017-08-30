+++
title = "Contact"
weight = 40
draft = false
+++

<form id="contactform" method="post" action="https://formspree.io/tatuhut@gmail.com">
	<div class="field half first">
		<input type="text" name="name" id="name" placeholder="Name"/>
	</div>
	<div class="field half">
		<input type="email" id="email" name="email" placeholder="Email">
	</div>
	<div class="field">
		<textarea name="message" id="message" rows="4" placeholder="Message"></textarea>
	</div>
	<ul class="actions">
		<li><input type="submit" value="Send message" class="special" /></li>
		<li><input type="reset" value="Reset" /></li>
	</ul>
	<input type="hidden" name="_next" value="?sent#contact" />
	<input type="hidden" name="_subject" value="Yhteydenotto" />
	<input type="text" name="_gotcha" style="display:none" />
</form>
<span id="contactformsent">Thank you for your message</span>

<script>
$(document).ready(function($) { 
    $(function(){
        if (window.location.search == "?sent") {
        	$('#contactform').hide();
        	$('#contactformsent').show();
        } else {
        	$('#contactformsent').hide();
        }
    });
});
</script>


{{< socialLinks >}}
