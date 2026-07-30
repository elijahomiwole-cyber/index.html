<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Waste Pickup Scheduler</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

<div class="container">

    <h1>🗑 Waste Pickup Scheduler</h1>
    <p>Schedule your waste pickup easily.</p>

    <!-- Dashboard -->
    <div class="dashboard">
        <div class="card">
            <h3>Total Pickups</h3>
            <p id="totalPickups">0</p>
        </div>

        <div class="card">
            <h3>Today's Pickups</h3>
            <p id="todayPickups">0</p>
        </div>

        <div class="card">
            <h3>Completed</h3>
            <p id="completedPickups">0</p>
        </div>

        <div class="card">
            <h3>Pending</h3>
            <p id="pendingPickups">0</p>
        </div>
    </div>

    <!-- Pickup Form -->
    <form id="pickupForm">

        <input
            type="text"
            id="name"
            placeholder="Full Name"
            required>

        <input
            type="tel"
            id="phone"
            placeholder="Phone Number"
            required>

        <textarea
            id="address"
            placeholder="Pickup Address"
            required></textarea>

        <select id="wasteType" required>
            <option value="">Select Waste Type</option>
            <option>Household Waste</option>
            <option>Plastic</option>
            <option>Paper</option>
            <option>Glass</option>
            <option>Metal</option>
            <option>Organic Waste</option>
        </select>

        <input
            type="date"
            id="date"
            required>

        <input
            type="time"
            id="time"
            required>

        <button type="submit">
            Schedule Pickup
        </button>

    </form>

    <!-- Search -->
    <input
        type="text"
        id="search"
        placeholder="Search by name, address or waste type">

    <!-- Filter -->
    <select id="statusFilter">
        <option value="all">All Pickups</option>
        <option value="pending">Pending</option>
        <option value="today">Due Today</option>
        <option value="completed">Completed</option>
    </select>

    <!-- Pickup List -->
    <h2>Scheduled Pickups</h2>

    <div id="pickupList"></div>

    <hr>

    <!-- Feedback -->
    <h2>Customer Feedback</h2>

    <input
        type="text"
        id="feedbackName"
        placeholder="Your Name">

    <select id="rating">
        <option value="">Select Rating</option>
        <option>⭐⭐⭐⭐⭐</option>
        <option>⭐⭐⭐⭐</option>
        <option>⭐⭐⭐</option>
        <option>⭐⭐</option>
        <option>⭐</option>
    </select>

    <textarea
        id="comment"
        placeholder="Leave your feedback"></textarea>

    <button onclick="saveFeedback()">
        Submit Feedback
    </button>

    <div id="feedbackList"></div>

    <footer>
        <hr>
        <p><strong>Waste Pickup Scheduler</strong></p>
        <p>Developed by Elijah Omiwole</p>
        <p>3MTT NextGen Project – 2026</p>
    </footer>

</div>

<script src="script.js"></script>

</body>
</html>
