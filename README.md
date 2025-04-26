<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sign in - Google Accounts</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
    <style>
        /* Custom styles for fine-tuning */
        body {
            font-family: 'Inter', sans-serif;
            background-color: #fff; /* Google's background is typically white */
            display: flex;
            flex-direction: column; /* Arrange items vertically */
            justify-content: center;
            align-items: center;
            min-height: 100vh; /* Center vertically */
            padding: 20px; /* Add some padding to the body */
        }
        .google-form-container {
            border: 1px solid #dadce0; /* Google's border color */
            border-radius: 8px; /* Google's border radius */
            padding: 48px 40px 36px; /* Google's padding */
            width:800px%;
            max-width: 450px; /* Max width similar to Google's form */
            box-shadow: 0 1px 3px 0 rgba(60,64,67,.3), 0 4px 8px 3px rgba(60,64,67,.15); /* Subtle Google-like shadow */
            margin-bottom: 24px; /* Space between form and footer */
        }
        .google-logo {
            width: 150px; /* Adjust logo size */
            margin-bottom: 24px; /* Space below logo */
        }
        .form-title {
            font-size: 24px; /* Title font size */
            margin-bottom: 8px; /* Space below title */
            text-align: center;
            color: #202124; /* Google's text color */
        }
        .form-subtitle {
            font-size: 16px; /* Subtitle font size */
            margin-bottom: 24px; /* Space below subtitle */
            text-align: center;
            color: #5f6368; /* Google's secondary text color */
        }
        .input-group {
            margin-bottom: 16px; /* Space between input groups */
        }
        .google-input {
            width: 100%;
            padding: 15px 15px; /* Input padding */
            border: 1px solid #dadce0; /* Input border color */
            border-radius: 4px; /* Input border radius */
            font-size: 16px; /* Input font size */
            box-sizing: border-box; /* Include padding and border in element's total width and height */
            transition: border-color 0.2s ease-in-out; /* Smooth border transition */
        }
        .google-input:focus {
            outline: none; /* Remove default outline */
            border-color: #1a73e8; /* Google's blue focus color */
            box-shadow: 0 1px 1px 0 rgba(26,115,232,.08); /* Subtle focus shadow */
        }
        .link-button {
            background: none;
            border: none;
            color: #1a73e8; /* Google's link color */
            font-size: 14px;
            padding: 0;
            cursor: pointer;
            text-align: left;
            margin-bottom: 24px; /* Space below link */
        }
        .link-button:hover {
            text-decoration: underline;
        }
        .button-group {
            display: flex;
            justify-content: space-between; /* Space out buttons */
            align-items: center;
            margin-top: 32px; /* Space above button group */
        }
        .create-account-button {
            background: none;
            border: none;
            color: #1a73e8; /* Google's link color */
            font-size: 14px;
            padding: 0;
            cursor: pointer;
        }
         .create-account-button:hover {
            text-decoration: underline;
        }
        .next-button {
            background-color: #1a73e8; /* Google's blue button color */
            color: #fff; /* White text */
            padding: 10px 24px; /* Button padding */
            border: none;
            border-radius: 4px; /* Button border radius */
            font-size: 14px;
            font-weight: 500; /* Medium font weight */
            cursor: pointer;
            transition: background-color 0.2s ease-in-out; /* Smooth background transition */
        }
        .next-button:hover {
            background-color: #1669ce; /* Darker blue on hover */
        }

  /* Footer styles */
        .google-footer {
            width: 100%;
            max-width: 450px; /* Match form width */
            display: flex;
            justify-content: space-between; /* Space out items */
            align-items: center;
            font-size: 12px; /* Smaller font size for footer */
            color: #5f6368; /* Google's secondary text color */
        }
        .google-footer a {
            color: #5f6368; /* Link color */
            text-decoration: none; /* No underline by default */
            margin-left: 16px; /* Space between links */
        }
        .google-footer a:hover {
            text-decoration: underline;
        }
        .language-selector select {
            border: none;
            background-color: transparent;
            font-size: 12px;
            color: #5f6368;
            cursor: pointer;
            outline: none;
        }
    </style>
</head>
<body>
    <div class="google-form-container">
        <div class="flex justify-center">
             <img src="https://www.google.com/images/branding/googlelogo/1x/googlelogo_color_272x92dp.png" alt="Google" class="google-logo">
        </div>

   <h1 class="form-title">Sign in</h1>
        <p class="form-subtitle">Use your Google Account</p>

 <form action="#" method="POST">
            <div class="input-group">
                <input type="text" id="email" name="email" class="google-input" placeholder="Email or phone">
            </div>

   <div class="input-group">
                 <input type="password" id="password" name="password" class="google-input" placeholder="Password">
            </div>

  <button type="button" class="link-button">Forgot email?</button>

   <div class="button-group">
                 <button type="button" class="create-account-button">Create account</button>
                 <button type="submit" class="next-button">Next</button>
            </div>
        </form>
    </div>
  <footer class="google-footer">
        <div class="language-selector">
            <select>
                <option value="en">English (United States)</option>
                <option value="es">Español</option>
                <option value="fr">Français</option>
            </select>
        </div>
        <div>
            <a href="#">Help</a>
            <a href="#">Privacy</a>
            <a href="#">Terms</a>
        </div>
    </footer>
</body>
</html>
