<script>
    let username = "gebruikersnaam";
    let usernameClicked = false;
    let password = "password";
    let passwordClicked = false

</script>

<body>
    <div class="login-card">
        <h1>Log hier in:</h1>
        <b>Gebruikersnaam: </b>
        <div>
            <input 
                on:click={() => {
                    if (!usernameClicked) {
                        usernameClicked = true
                        username = ""
                    }
                }} 
                type="text" bind:value={username} 
                label="gebruikersnaam"
            />
        </div>
        <b>Password: </b>
        <div>
            <input 
                on:click={() => {
                    if (!passwordClicked) {
                        passwordClicked = true
                        password = ""
                    }
                }} 
                type="password" bind:value={password} 
                label="password"
            />
        </div>
        <button on:click={alert("Username: " + username + "\n" + "Password: " + password )}>Log in</button>
        
    </div>
</body>

<style>

    body {
        align-items: center;
        box-sizing: border-box;
        display: flex;
        flex-direction: column;
    }

    .login-card {
        border-radius: 20px;
        display: flex;
        flex-direction: column;
        align-items: center;
        background-color: antiquewhite;
        width: 40%;
    }

</style>