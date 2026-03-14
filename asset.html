<?php
include("db_connect.php"); 

$fullname = $_POST['fullname'];
$phone_no = $_POST['phone_no'];
$room = $_POST['room'];
$mtstay = $_POST['mtstay'];
$add_ms = $_POST['add_ms'];
$code = $_POST['code'];
$haddress = $_POST['haddress'];
$room_no = $_POST['room_no'];

// Sanitize inputs to prevent SQL injection
$fullname = mysqli_real_escape_string($conn, $fullname);
$phone_no = mysqli_real_escape_string($conn, $phone_no);
$room = mysqli_real_escape_string($conn, $room);
$mtstay = mysqli_real_escape_string($conn, $mtstay);
$add_ms = mysqli_real_escape_string($conn, $add_ms);
$code = mysqli_real_escape_string($conn, $code);
$haddress = mysqli_real_escape_string($conn, $haddress);
$room_no = mysqli_real_escape_string($conn, $room_no);

$query = mysqli_query($conn, "INSERT INTO live_form 
    (fullname, phone_no, room, mtstay, add_ms, code, haddress, room_no) 
    VALUES ('$fullname', '$phone_no', '$room', '$mtstay', '$add_ms', '$code', '$haddress', '$room_no')");

if ($query) {
    $success = true;
    $reservationCode = $code;
} else {
    $success = false;
    $error = mysqli_error($conn);
}

mysqli_close($conn); 
?>

<!doctype html>
<html lang="en">
<head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Reservation Status | Janet's Haven</title>
    
    <!-- Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    
    <!-- Icons -->
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.0/font/bootstrap-icons.css">
    
    <!-- Custom CSS -->
    <link href="css/futuristic.css" rel="stylesheet">
    
    <style>
        body {
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            background: var(--primary-bg);
        }
        
        .status-card {
            background: var(--glass-bg);
            backdrop-filter: blur(30px);
            border: 1px solid var(--glass-border);
            border-radius: 30px;
            padding: 60px;
            text-align: center;
            max-width: 500px;
            width: 90%;
            position: relative;
            overflow: hidden;
        }
        
        .status-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 4px;
            background: <?php echo $success ? 'var(--gradient-primary)' : 'linear-gradient(90deg, #ff4444, #ff8844)'; ?>;
        }
        
        .status-icon {
            width: 100px;
            height: 100px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 0 auto 30px;
            font-size: 3rem;
            <?php if ($success): ?>
            background: var(--gradient-primary);
            box-shadow: 0 10px 40px rgba(0, 245, 255, 0.4);
            <?php else: ?>
            background: linear-gradient(135deg, #ff4444, #ff8844);
            box-shadow: 0 10px 40px rgba(255, 68, 68, 0.4);
            <?php endif; ?>
        }
        
        .status-icon i {
            color: white;
        }
        
        .status-card h2 {
            font-size: 2rem;
            margin-bottom: 15px;
        }
        
        .status-card p {
            color: var(--text-secondary);
            margin-bottom: 30px;
        }
        
        .reservation-code {
            background: rgba(0, 245, 255, 0.1);
            border: 1px solid rgba(0, 245, 255, 0.3);
            border-radius: 15px;
            padding: 20px;
            margin: 25px 0;
        }
        
        .reservation-code label {
            display: block;
            color: var(--neon-cyan);
            font-size: 0.9rem;
            margin-bottom: 10px;
        }
        
        .reservation-code .code {
            font-size: 2.5rem;
            font-weight: 700;
            color: var(--text-primary);
            letter-spacing: 8px;
            font-family: monospace;
        }
        
        .btn-group {
            display: flex;
            gap: 15px;
            justify-content: center;
            flex-wrap: wrap;
        }
        
        .btn {
            min-width: 150px;
        }
        
        @media (max-width: 480px) {
            .status-card {
                padding: 40px 25px;
            }
            
            .reservation-code .code {
                font-size: 1.8rem;
                letter-spacing: 5px;
            }
        }
    </style>
</head>
<body>
    <!-- Background Effects -->
    <div class="bg-grid"></div>
    <div class="orb orb-1"></div>
    <div class="orb orb-2"></div>

    <div class="status-card">
        <?php if ($success): ?>
            <div class="status-icon">
                <i class="bi bi-check-lg"></i>
            </div>
            <h2>Reservation <span style="background: var(--gradient-primary); -webkit-background-clip: text; -webkit-text-fill-color: transparent;">Successful!</span></h2>
            <p>Thank you for choosing Janet's Haven. Your reservation has been submitted successfully.</p>
            
            <div class="reservation-code">
                <label><i class="bi bi-shield-lock"></i> Your Reservation Code</label>
                <div class="code"><?php echo htmlspecialchars($reservationCode); ?></div>
                <small style="color: var(--text-muted);">Save this code for future reference</small>
            </div>
            
            <p style="font-size: 0.9rem;">We will contact you shortly to confirm your reservation.</p>
            
            <div class="btn-group">
                <a href="index.php" class="btn btn-primary btn-glow">
                    <i class="bi bi-house"></i> Back to Home
                </a>
                <a href="ticket.php" class="btn btn-secondary">
                    <i class="bi bi-plus-lg"></i> New Reservation
                </a>
            </div>
        <?php else: ?>
            <div class="status-icon" style="background: linear-gradient(135deg, #ff4444, #ff8844);">
                <i class="bi bi-x-lg"></i>
            </div>
            <h2>Reservation <span style="color: #ff4444;">Failed</span></h2>
            <p>We encountered an error while processing your reservation. Please try again.</p>
            
            <?php if (isset($error)): ?>
                <div style="background: rgba(255, 68, 68, 0.1); border: 1px solid rgba(255, 68, 68, 0.3); border-radius: 10px; padding: 15px; margin: 20px 0; color: #ff8888; font-size: 0.85rem;">
                    <i class="bi bi-exclamation-triangle"></i> Error: <?php echo htmlspecialchars($error); ?>
                </div>
            <?php endif; ?>
            
            <div class="btn-group">
                <a href="javascript:history.back()" class="btn btn-secondary">
                    <i class="bi bi-arrow-left"></i> Go Back
                </a>
                <a href="index.php" class="btn btn-primary" style="background: linear-gradient(135deg, #ff4444, #ff8844);">
                    <i class="bi bi-house"></i> Back to Home
                </a>
            </div>
        <?php endif; ?>
    </div>

    <script>
        // Auto-redirect after 10 seconds on success
        <?php if ($success): ?>
        setTimeout(function() {
            window.location.href = 'index.php';
        }, 10000);
        <?php endif; ?>
    </script>
</body>
</html>
