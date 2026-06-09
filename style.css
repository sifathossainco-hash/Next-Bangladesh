// Function to show current date in Bangla
function updateDate() {
    const options = { weekday: 'long', year: 'numeric', month: 'long', day: 'numeric' };
    const today = new Date();
    
    // Using Intl.DateTimeFormat for Bangla locale
    const formatter = new Intl.DateTimeFormat('bn-BD', options);
    const parts = formatter.formatToParts(today);
    
    // Adding some additional formatting for a premium look
    document.getElementById('current-date').innerText = 
        `আজ: ${formatter.format(today)}`;
}

// Dark Mode Toggle
const themeToggle = document.getElementById('theme-toggle');
const body = document.body;
const icon = themeToggle.querySelector('i');

themeToggle.addEventListener('click', () => {
    body.classList.toggle('dark-mode');
    
    // Switch icons
    if (body.classList.contains('dark-mode')) {
        icon.classList.remove('fa-moon');
        icon.classList.add('fa-sun');
        localStorage.setItem('theme', 'dark');
    } else {
        icon.classList.remove('fa-sun');
        icon.classList.add('fa-moon');
        localStorage.setItem('theme', 'light');
    }
});

// Check for saved theme preference
window.onload = () => {
    updateDate();
    
    const savedTheme = localStorage.getItem('theme');
    if (savedTheme === 'dark') {
        body.classList.add('dark-mode');
        icon.classList.remove('fa-moon');
        icon.classList.add('fa-sun');
    }
};

// Navbar shadow on scroll
window.addEventListener('scroll', () => {
    const nav = document.querySelector('.main-nav');
    if (window.scrollY > 50) {
        nav.classList.add('shadow');
    } else {
        nav.classList.remove('shadow');
    }
});
