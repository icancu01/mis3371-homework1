  /* Place your JavaScript in this file */
// Program name: script.js
// Author: Si John Van
// Date created: 2024-09-25
// Date Modified: 2024-09-25
// Version: 1.0
// Description: This file provides the dynamic time for banner  -->


function updateDateTime() {
    const now = new Date();

    const options = {
        weekday: 'long',
        year: 'numeric',
        month: 'long',
        day: 'numeric',
        hour: 'numeric',
        minute: 'numeric',
        second: 'numeric',
        hour12: true
    }

    const formattedDateTime = now.toLocaleString(undefined, options);
    document.getElementById("datetime").textContent = "Today's date is: " + formattedDateTime;

}

updateDateTime();

setInterval(updateDateTime, 1000);
