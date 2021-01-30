<script>
    let username = "gebruikersnaam";
    let usernameClicked = false;
    let email = "example@provider.pog";
    let emailClicked = false;
    let password = "password";
    let passwordClicked = false;
    let repassword = "re-enter password";
    let repasswordClicked = false;

</script>

<body>
    <div class="login-card">
        <h1>Maak een account aan:</h1>
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
            />
        </div>
        <b>E-Mail</b>
        <div>
            <input 
                on:click={() => {
                    if (!emailClicked) {
                        emailClicked = true
                        email = ""
                    }
                }} 
                type="text" bind:value={email} 
            />
        </div>
        <b>Wachtwoord: </b>
        <div>
            <input 
                on:click={() => {
                    if (!passwordClicked) {
                        passwordClicked = true
                        password = ""
                    }
                }} 
                type="password" bind:value={password}
            />
        </div>
        <b>Herhaal wachtwoord: </b>
        <div>
            <input 
                on:click={() => {
                    if (!repasswordClicked) {
                        repasswordClicked = true
                        repassword = ""
                    }
                }} 
                type="password" bind:value={repassword}
            />
        </div>
        <button on:click={alert(
            "Username: " + username + "\n" + 
            "email: " + email + "\n" +
            "Password: " + password + "\n"
            )}>
            Log in
        </button>
        
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