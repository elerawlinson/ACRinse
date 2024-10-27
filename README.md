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

<h2>How to Use the Program:</h2>

<div style="background-color: #e7f3fe; padding: 10px; border-left: 6px solid #2196F3; margin-bottom: 20px;">
    <p>To see the server working, refer to: <a href="https://drive.google.com/drive/folders/1e9ylJGAOr75ZgmvuFBOb8s8uLiDJ_Lrg?usp=sharing" target="_blank">Google Drive</a></p>
</div>

<ul>
    <li>For all of the buttons and interfaces of the app, the main way to work your way through it is by using mouse clicks.</li>
    <li>The program will ask you to log in or register. To log in, the program only needs an email as input, which you will write in the textbox in the panel. If the account is found, it will log in as the user with that email. Otherwise, you can create a new user by providing a name, last name, and email address, which will create a new account and store it in the data.</li>
    <li>The program opens on the home page, and the user can select any of the following buttons:
        <ul>
            <li><strong>Your Profile</strong>: View your information, bubbles, current machine status, and all-time total loads and overtime (late) loads.</li>
            <li><strong>Washing Tips</strong>: Promote good washing behavior that benefits everyone (and the environment!).</li>
            <li><strong>Home</strong>: Returns to the home page.</li>
            <li><strong>Leaderboard</strong>: Shows the top 10 users with the most bubbles to incentivize good washing machine etiquette. Bubbles will change depending on how many loads you complete or how late you are to take your loads from the machines. You gain 100 bubbles for completing a load and lose bubbles for picking it up late.</li>
            <li><strong>Machine Status</strong>: See the status of every washer and dryer: red if occupied, yellow if pending, and green if available.</li>
            <li><strong>Put a Load In</strong>: Shows you available washers. After washing, a button will appear to take you to the dryer page. If a machine is pending and the owner doesn't take their load, they have a 10-minute grace period before anyone can take their clothes out.</li>
            <li><strong>Queue</strong>: A FIFO linked list that users can join if all machines are taken. There’s a queue for both washers and dryers.</li>
            <li><strong>Data Handling</strong>: All data regarding machine availability is based on a JSON file (ACRinse.txt). Our program updates machine statuses based on this data, which is constantly synchronized with a server.</li>
            <li><strong>Using the Server</strong>: Have a copy of ACRinse.txt in the <code>src</code> folder. Compile normally. To connect to a server from a client thread, use “localhost” and add the IP address of the computer running the server, ensuring the same port number (6066). Uncomment necessary parts of the code as indicated.</li>
        </ul>
    </li>
</ul>


