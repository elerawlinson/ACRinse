Amr Al Dayeh, Elena Rawlinson, Javier Gutierrez Bach 
COSC 112 

<h2>To Run the Program</h2>
<ul>
    <li>Note: You need to have Java installed on your local machine.</li>
    <li>Download ACRinse folder</li>
    <li>Download Project.Java/src that should contain:
        <ul>
            <li>Project.java</li>
            <li>All images</li>
            <li>ACRinse.txt</li>
            <li>json-simple-1.1.jar</li>
        </ul>
    </li>
    <li>From terminal, cd into ACRinse</li>
    <li>Run the following commands:</li>
        <ul>
    <li><code>javac -cp .:json-simple-1.1.1.jar Project.java</code></li>
    <li><code>java -cp .:json-simple-1.1.1.jar Project</code></li>
        </ul>

</ul>

<h2>How to use the program:</h2>
<ul>
    <li>To see the server working, refer to: https://drive.google.com/drive/folders/1e9ylJGAOr75ZgmvuFBOb8s8uLiDJ_Lrg?usp=sharing</li>
    <li>For all of the buttons and interfaces of the app, the main way to work your way through it is by using the mouse click.</li>
    <li>First up, the program will ask you to log in or register. To log in, the program only needs an email as an input, which you will write on the textbox in the panel, and then if the account is found, it will log in as the user with that email. Otherwise, you can create a new user and give it a name, last name, and an email address which will create a new account and store it in the data.</li>
    <li>The program opens on the home page and the user can select any of the following buttons:
        <ul>
            <li>Your profile - you can see your information, bubbles, your current machine status, and your all-time total loads and overtime (late) loads.</li>
            <li>Washing Tips - to promote good washing behavior that benefits everyone (and the environment!).</li>
            <li>Home - returns to the home page.</li>
            <li>Queue - explained below.</li>
            <li>Leaderboard - shows the top 10 users with the most bubbles to incentivize good washing machine etiquette. Bubbles will change depending on how many loads you complete or how late you are to take your loads from the machines. If you complete a load in any machine, you will get 100 bubbles. If you pick it up more than 10 minutes late, you will lose 15 bubbles. An hour late → lose 100 bubbles. 3 hours late → lose 200 bubbles. A day late → lose 500 bubbles.</li>
            <li>Machine status - You can see the status of every washer and dryer. It will be red if occupied, with the name of the user occupying it and the time remaining. It will be yellow if it is pending, meaning the load is ready but hasn't been taken out of the machine. Finally, if it is green, then the machine is available.</li>
            <li>Put a load in - This page shows you the washers, and if there is a machine available and you do not have a load in already, then you can put a load in said machine. Once you have washed a load, a button will appear on the button that takes you to the dryer page, which works similarly to the washer page. If a machine is pending but the owner doesn't take their load, then they will have a 10-minute grace period to get their clothes, and after that period, anyone can take their clothes off in the app (and hopefully in real life too).</li>
            <li>Queue - The queue is a FIFO linked list we made that users can join in the queue page of the app. This works so that if you really want to wash and all the machines are taken, then you can join the queue. We have a queue for both the dryers and the washers.</li>
            <li>All of the data regarding machine availability is determined by data we created (fake users, emails, load availability) which is written in a JSON file (the file you downloaded, called ACRinse.txt). Our program takes the information from the JSON file and updates the machine statuses/availability accordingly. This data is constantly updated with a server that runs simultaneously as many users, and the data gets sent and received by all of the users, so that you can see in your app what other users do.</li>
            <li>To use the server: have a copy of ACRinse.txt in the src file and compile normally, if you want to connect to a server from a client thread, command f “localhost” in the project file and then add the IP address of the computer the server is running on and make sure you have the same number as port for the server and client (should be 6066). You also need to uncomment all the parts of the code that are commented (in the main method, writeJson method, and the while(true) loop in runner). You can find "uncomment" above each snippet that needs to be uncommented.</li>
        </ul>
    </li>
</ul>
