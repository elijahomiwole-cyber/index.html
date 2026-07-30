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

    <header>
        <h1>🗑 Waste Pickup Scheduler</h1>

        <p class="subtitle">
            Schedule waste pickups quickly and easily. Track pickup requests,
            receive reminders, and submit feedback to improve waste management.
        </p>
    </header>

    <!-- Dashboard -->
    <section class="dashboard">

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

    </section>

    <!-- Schedule Form -->

    <section>

        <h2>Schedule a Waste Pickup</h2>

        <form id="pickupForm">

            <label for="name">Full Name</label>

            <input
                type="text"
                id="name"
                placeholder="Enter your full name"
                required>

            <label for="phone">Phone Number</label>

            <input
                type="tel"
                id="phone"
                placeholder="Enter your phone number"
                required>

            <label for="address">Pickup Address</label>

            <textarea
                id="address"
                placeholder="Enter pickup address"
                required></textarea>

            <label for="wasteType">Waste Type</label>

            <select id="wasteType" required>

                <option value="">Select Waste Type</option>

                <option>Household Waste</option>

                <option>Plastic</option>

                <option>Paper</option>

                <option>Glass</option>

                <option>Metal</option>

                <option>Organic Waste</option>

            </select>

            <label for="date">Pickup Date</label>

            <input
                type="date"
                id="date"
                required>

            <label for="time">Pickup Time</label>

            <input
                type="time"
                id="time"
                required>

            <button type="submit">
                Schedule Pickup
            </button>

        </form>

    </section>
