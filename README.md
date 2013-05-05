arrayctl
=========

<dt>Cubescript Array Controler (FAQ)</dt>
-------------------------
<dt>What's arrayctl for?</dt>
Dynamic client / server script's which require to save data fast and effective.
For example arrayctl can be used to give every player certain settings or count special values

<dt>How does it work?</dt>
-------------------------
Let's get started, you NEED to setup the element's array, all other options are pre-filled and may be changed.
After you setted up your ```element tree``` you are ready for use.

	(for example like this: kills jumps suicides)

<dt>Example script</dt>

	values = "3 10 1" //In this case, 3 kills, 10 jumps, 1 suicide
	addEntry $cn $values //lets add the values
	delEntry $cn //if user leaves

So what if we need to know a user's frags? That's easy!:

	frags = (getEntryDetail $cn kills)
	
You might need to change the user's value too:

	changeEntryDetail $cn kills $newkills //Assign a new value for cn

Isn't that awesome :P?!
If you need anything or know something to improve just pull, or contact me: fohlen@opencoop.net
