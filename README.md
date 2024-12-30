<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Smart Package Vault</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="container">
        <h1>Smart Package Vault</h1>
        <p>Be smart, Secure Packages</p>

        <!-- Vault Status -->
        <div id="vaultStatus" class="status">Status: Locked</div>

        <!-- PIN Entry -->
        <div>
            <label for="pinInput">Enter PIN to Open Package Vault:</label>
            <input type="password" id="pinInput" placeholder="Enter PIN">
        </div>
        <button id="unlockButton" class="btn">Unlock</button>
        <button id="lockButton" class="btn">Lock</button>
        <button id="resetButton" class="btn">Reset PIN</button>

        <!-- Reset PIN Section (Initially Hidden) -->
        <div id="resetPinSection" style="display: none;">
            <h2>Reset PIN</h2>
            <p>If you have forgotten your PIN, choose one of the following options:</p>

            <div id="previousPinOption">
                <label for="previousPin">Enter Previous PIN:</label>
                <input type="password" id="previousPin" placeholder="Enter Previous PIN">
                <button id="verifyPreviousPin" class="btn">Verify Previous PIN</button>
            </div>

            <div id="backupQuestionsOption">
                <p>Or answer the backup questions:</p>
                <label for="backupQuestion1">What is your mother's maiden name?</label>
                <input type="text" id="backupQuestion1">
                <label for="backupQuestion2">What was your first pet's name?</label>
                <input type="text" id="backupQuestion2">
                <button id="verifyBackupQuestions" class="btn">Verify Answers</button>
            </div>
        </div>

        <!-- Reset Status -->
        <div id="resetStatus"></div>
    </div>

    <script src="scripts.js"></script>
</body>
</html>
