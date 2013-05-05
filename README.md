arrayctl
=========

<h2>Cubescript Array Controler (FAQ)<h2>
<h3>What's arrayctl for?</h3>
<p>Dynamic client / server script's which require to save data fast and effective.
For example arrayctl can be used to give every player certain settings or count special values</p>
<h3>How does it work?</h3>
<p>Let's get started, you NEED to setup the element's array, all other options are pre-filled and may be changed.
After you setted up your element tree (for example like this: ```kills jumps suicides```) you are ready for use.</p>
<table>
<tr>Example script</tr>
<td>```values = "3 10 1" //In this case, 3 kills, 10 jumps, 1 suicide```</td>
<td>```addEntry $cn $values //lets add the values```</td>
<td>```delEntry $cn``` //if user leaves```</td>
</tr>
</table>
<p>So what if we need to know a user's frags? That's easy!:</br>
```frags = (getEntryDetail $cn kills)```</br>
You might need to change the user's value too:</br>
```changeEntryDetail $cn kills $newkills``` //Assign a new value for cn</br>
</br>
Isn't that awesome :P?!
</p>
