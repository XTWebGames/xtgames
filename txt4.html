// Initialize spikes array
let spikes = [];

// Function to generate random number of spikes (1 or 2)
function generateSpikes() {
    let numberOfSpikes = Math.floor(Math.random() * 2) + 1;  // Generates 1 or 2 spikes
    spikes = [];  // Clear existing spikes

    // Randomly generate positions for the spikes
    for (let i = 0; i < numberOfSpikes; i++) {
        let spikeX = canvas.width + Math.random() * 500;  // Random initial x position
        let spikeY = canvas.height - 50;  // Y position is always near the bottom
        let spikeWidth = 50;  // Width of each spike
        spikes.push({ x: spikeX, y: spikeY, width: spikeWidth, height: 50, speed: 5 });
    }
}

// Initialize score
let score = 0;

// Main game loop
function gameLoop() {
    // Draw background image
    ctx.drawImage(backgroundImage, 0, 0, canvas.width, canvas.height);

    player.update();
    player.draw();

    // Update and draw all spikes
    spikes.forEach(spike => {
        spike.x -= spike.speed;
        if (spike.x + spike.width < 0) {
            spike.x = canvas.width;
        }

        ctx.beginPath();
        ctx.moveTo(spike.x, spike.y + spike.height);
        ctx.lineTo(spike.x + spike.width / 2, spike.y);
        ctx.lineTo(spike.x + spike.width, spike.y + spike.height);
        ctx.fillStyle = 'black';
        ctx.fill();
    });

    // Draw score
    ctx.fillStyle = 'white';
    ctx.font = '20px Arial';
    ctx.fillText('Score: ' + score, 20, 40);

    // Check if player successfully jumped over any spike
    spikes.forEach(spike => {
        if (player.x > spike.x + spike.width && player.x < spike.x + spike.width + spike.speed) {
            score++;
        }

        // Check for collisions with each spike
        if (isColliding(player, spike)) {
            alert("Game Over! Score: " + score);
            document.location.reload();
        }
    });

    requestAnimationFrame(gameLoop);
}

// Collision detection function
function isColliding(rect1, rect2) {
    return rect1.x < rect2.x + rect2.width &&
           rect1.x + rect1.width > rect2.x &&
           rect1.y < rect2.y + rect2.height &&
           rect1.y + rect1.height > rect2.y;
}

// Event listener for jumping on click or tap
canvas.addEventListener('click', function() {
    player.jump();
});

// Start the game loop when images are loaded
backgroundImage.onload = playerImage.onload = function() {
    generateSpikes();  // Generate spikes when the game starts
    gameLoop();
};

// Resize canvas when window size changes
window.addEventListener('resize', function() {
    canvas.width = window.innerWidth;
    canvas.height = window.innerHeight;
    generateSpikes();  // Re-generate spikes when window is resized
});
