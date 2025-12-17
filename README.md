# HTTPS-www.Chase.com
Bank profile affiliated with chase bank only 
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Chase Bank Profile - Educational Only</title>
  <style>
    body {
      font-family: 'Segoe UI', Arial, sans-serif;
      background-color: #f4f6f9;
      margin: 0;
      padding: 0;
      color: #333;
    }
    header {
      background-color: #004b87;
      color: white;
      padding: 20px;
      text-align: center;
      box-shadow: 0 2px 10px rgba(0,0,0,0.1);
    }
    header h1 {
      margin: 0;
      font-size: 28px;
    }
    .disclaimer {
      background-color: #ffebcd;
      color: #856404;
      padding: 10px;
      text-align: center;
      font-weight: bold;
    }
    .container {
      max-width: 900px;
      margin: 30px auto;
      padding: 20px;
      background: white;
      border-radius: 10px;
      box-shadow: 0 4px 15px rgba(0,0,0,0.1);
    }
    .profile-section {
      display: flex;
      align-items: center;
      margin-bottom: 40px;
    }
    .profile-pic {
      width: 150px;
      height: 150px;
      border-radius: 50%;
      object-fit: cover;
      border: 4px solid #004b87;
      margin-right: 30px;
    }
    .profile-info h2 {
      margin: 0 0 10px 0;
      color: #004b87;
    }
    .upload-btn {
      background-color: #004b87;
      color: white;
      padding: 10px 20px;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      margin-top: 15px;
    }
    .upload-btn:hover {
      background-color: #003b6b;
    }
    .section {
      margin-bottom: 30px;
      padding: 20px;
      background-color: #f8f9fa;
      border-radius: 8px;
    }
    .section h3 {
      color: #004b87;
      border-bottom: 2px solid #004b87;
      padding-bottom: 8px;
    }
    .info-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 15px;
    }
    .info-item {
      background: white;
      padding: 15px;
      border-radius: 6px;
      box-shadow: 0 1px 5px rgba(0,0,0,0.05);
    }
    footer {
      text-align: center;
      padding: 20px;
      color: #666;
      font-size: 14px;
    }
  </style>
</head>
<body>
  <header>
    <h1>Chase Bank</h1>
  </header>

  <div class="disclaimer">
     AFFILIATED WITH CHASE BANK 
  </div>

  <div class="container">
    <div class="profile-section">
      <img id="profileImage" src="https://via.placeholder.com/150/004b87/white?text=IL" alt="Profile Picture" class="profile-pic">
      <div class="profile-info">
        <h2>Welcome, Ike Lewis</h2>
        <p>Member since: December 2025</p>
        <label class="upload-btn">
          Upload Profile Picture
          <input type="file" id="upload" accept="image/*" style="display:none;">
        </label>
      </div>
    </div>

    <div class="section">
      <h3>Login Information (Demo Only)</h3>
      <div class="info-grid">
        <div class="info-item">
          <strong>Username:</strong> IkeLewis2025
        </div>
        <div class="info-item">
          <strong>Password Hint:</strong> •••••••• (Never share real passwords)
        </div>
        <div class="info-item">
          <strong>Last Login:</strong> December 17, 2025
        </div>
      </div>
    </div>

    <div class="section">
      <h3>Account Overview (Simulated Data)</h3>
      <div class="info-grid">
        <div class="info-item">
          <strong>Checking Account</strong><br>
          Ending in ****1234<br>
          Balance: $5,234.56
        </div>
        <div class="info-item">
          <strong>Savings Account</strong><br>
          Ending in ****5678<br>
          Balance: $12,890.00
        </div>
      </div>
    </div>
  </div>

  <footer>
    This is a student educational project for learning web development.<br>
    Real banking services are available at <a href="https://www.chase.com" target="_blank">chase.com</a>
  </footer>

  <script>
    document.getElementById('upload').addEventListener('change', function(e) {
      if (e.target.files && e.target.files[0]) {
        const reader = new FileReader();
        reader.onload = function(ev) {
          document.getElementById('profileImage').src = ev.target.result;
        };
        reader.readAsDataURL(e.target.files[0]);
      }
    });
  </script>
</body>
</html>
