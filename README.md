# PWWTechnotice
PWW334 Tech notices
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Porsche Westwood – Message Board</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
    body {
        font-family: Arial, Helvetica, sans-serif;
        background: #f4f4f4;
        margin: 0;
        padding: 0;
        color: #222;
    }

    .header {
        background: #000;
        color: white;
        padding: 20px;
        text-align: center;
        border-bottom: 4px solid #b30000;
    }
    .header h1 {
        margin: 0;
        font-size: 26px;
        letter-spacing: 1px;
    }
    .header h2 {
        margin: 5px 0 0;
        font-size: 16px;
        font-weight: 300;
        opacity: 0.8;
    }

    .container {
        max-width: 900px;
        margin: 20px auto;
        padding: 0 15px;
    }

    .notice {
        background: white;
        border-radius: 8px;
        padding: 15px 20px;
        margin-bottom: 15px;
        border-left: 6px solid #ccc;
        box-shadow: 0 2px 4px rgba(0,0,0,0.1);
        cursor: pointer;
        transition: 0.2s;
    }
    .notice:hover {
        transform: scale(1.01);
    }

    .priority-critical { border-left-color: #d40000; }
    .priority-high { border-left-color: #ff9900; }
    .priority-normal { border-left-color: #0077cc; }

    .notice-title {
        font-size: 18px;
        font-weight: bold;
        margin-bottom: 6px;
    }

    .meta {
        font-size: 13px;
        color: #555;
        margin-bottom: 10px;
    }

    .tag {
        display: inline-block;
        padding: 3px 8px;
        font-size: 12px;
        border-radius: 4px;
        background: #eee;
        margin-right: 8px;
        text-transform: uppercase;
        font-weight: bold;
    }

    .content {
        display: none;
        margin-top: 10px;
        font-size: 15px;
        line-height: 1.5;
    }

    .notice.open .content {
        display: block;
    }
</style>

<script>
    document.addEventListener("DOMContentLoaded", function() {
        document.querySelectorAll(".notice").forEach(function(card) {
            card.addEventListener("click", function() {
                this.classList.toggle("open");
            });
        });
    });
</script>

</head>
<body>

<div class="header">
    <h1>Porsche Westwood</h1>
    <h2>Service & Dealer Message Board</h2>
</div>

<div class="container">

    <!-- SAMPLE NOTICE (Replace with backend data) -->
    <div class="notice priority-critical">
        <div class="notice-title">ASB2 Stop Delivery – Immediate Action Required</div>
        <div class="meta">
            <span class="tag">Recalls</span>
            Posted Feb 26, 2026 • Expires Mar 15, 2026
        </div>
        <div class="content">
            <p>This is placeholder content. Your backend will insert TinyMCE‑formatted HTML here.</p>
        </div>
    </div>

    <div class="notice priority-high">
        <div class="notice-title">New PIWIS Tester Software Update</div>
        <div class="meta">
            <span class="tag">Tools</span>
            Posted Feb 25, 2026
        </div>
        <div class="content">
            <p>Details about the new PIWIS update go here.</p>
        </div>
    </div>

    <div class="notice priority-normal">
        <div class="notice-title">Weekly Dealership Update</div>
        <div class="meta">
            <span class="tag">General</span>
            Posted Feb 24, 2026
        </div>
        <div class="content">
            <p>General dealership announcements appear here.</p>
        </div>
    </div>

</div>

</body>
</html>
