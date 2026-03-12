function openInquiryForm() {
    document.getElementById("inquiry-form").style.display = "flex";
}

function closeInquiryForm() {
    document.getElementById("inquiry-form").style.display = "none";
}

function scrollToSection(sectionId) {
    const section = document.getElementById(sectionId);
    if (section) {
        section.scrollIntoView({ behavior: 'smooth' });
    }
}
function searchPlaces() {
    // Get the search input value
    const searchInput = document.querySelector('.search-bar input').value.toLowerCase();
    
    // Get all tour cards
    const tourCards = document.querySelectorAll('.tour-card');

    // Loop through each tour card and check if it matches the search input
    tourCards.forEach(card => {
        const tourName = card.querySelector('.tour-details h3').innerText.toLowerCase();
        if (tourName.includes(searchInput)) {
            card.style.display = ''; // Show the card if it matches
        } else {
            card.style.display = 'none'; // Hide the card if it doesn't match
        }
    });
}
function openModal(id) {
    document.getElementById(id).style.display = 'flex';
}

function closeModal(id) {
    document.getElementById(id).style.display = 'none';
}


function viewDetails(tourName) {
    const details = {
        "Dwarka Tour": "Explore the sacred city of Dwarka, known for its rich history and beautiful temples. Dwarka, one of the Char Dhams, is a sacred city located on the western tip of Gujarat. It’s known for the Dwarkadhish Temple, dedicated to Lord Krishna. This ancient city is steeped in mythology and offers spiritual vibes, beautiful temples, and serene coastal views.Duration: 3 Nights / 4 Days. Visit the Dwarkadhish Temple, Nageshwar Jyotirlinga, and enjoy local cuisine.",
        "Temple Somnath": "Visit the famous Somnath Temple, one of the twelve Jyotirlingas of Lord Shiva. The Somnath Temple, located in Prabhas Patan near Veraval, is one of the twelve Jyotirlingas of Lord Shiva. It has been destroyed and rebuilt several times in history and stands today as a symbol of eternal faith and architectural brilliance, right on the Arabian Sea coast.Duration: 4 Nights / 5 Days. Experience the evening aarti and explore nearby attractions.",
        "gir national park": "Discover the wildlife of Sasan Gir National Park, home to the Asiatic lion.Gir National Park, located near Junagadh, is the only natural habitat of Asiatic Lions in the world. It’s a major wildlife attraction with safaris, bird watching, and eco-tourism activities, attracting nature and wildlife lovers. Duration: 2 Nights / 3 Days. Enjoy safari rides and nature walks in this beautiful sanctuary.",
        "Mandvi": "Relax on the beautiful beaches of Mandvi, known for its stunning coastline and historical sites.Mandvi is a charming town in Kutch, known for its clean and peaceful Mandvi Beach. The beach offers camel rides, water sports, and scenic sunsets. The Vijay Vilas Palace, nearby, adds a royal touch to the visit. Duration: 2 Nights / 3 Days. Visit the Vijay Vilas Palace and enjoy water sports.",
        "Saputara Hill Station": "Experience the lush greenery and cool climate of Saputara Hills, a popular hill station.Saputara is Gujarat’s only hill station, nestled in the Sahyadri Hills. It offers cool weather, lush greenery, boating in Saputara Lake, ropeways, gardens, tribal culture, and trekking spots—perfect for a relaxing getaway. Duration: 2 Nights / 3 Days. Enjoy boating on Saputara Lake and visit the Sunset Point.",
        "Champaner": "Explore the UNESCO World Heritage Site of Champaner, known for its historical forts and temples.This UNESCO World Heritage Site includes Champaner, an ancient city with stunning Indo-Islamic architecture, and Pavagadh Hill, crowned with the famous Kalikamata Temple. It’s a unique blend of archaeology, history, and spirituality. Duration: 1 Night / 2 Days. Visit the Pavagadh Fort and ancient mosques.",
        "Kutch": "Discover the unique culture and landscapes of Kutch, famous for its white salt desert. Kutch is known for the spectacular Rann of Kutch, a white salt desert that comes alive during the Rann Utsav with folk music, dance, handicrafts, and tent city stays. It’s also home to beautiful villages, palaces, and rich Kutchi culture.Duration: 3 Nights / 4 Days. Experience the Rann Utsav and visit local handicraft villages.",
        "Statue of Unity": "Experience the vibrant culture and traditions of Gujarat through the Sou tour.Located near the Sardar Sarovar Dam, the Statue of Unity is the world’s tallest statue, dedicated to Sardar Vallabhbhai Patel. It’s surrounded by a museum, laser light shows, valley of flowers, and offers panoramic views from the viewing gallery. Duration: 2 Nights / 3 Days. Visit local markets, taste authentic cuisine, and enjoy folk performances."
    };

    alert(details[tourName] || "Details not available.");
}

function bookingRequest(tourName) {
    const bookingForm = `
        <div class="modal-content">
            <span class="close" onclick="closeBookingForm()">&times;</span>
            <h2>Booking Request for ${tourName}</h2>
            <form id="booking-form">
                <input type="text" placeholder="Your Name" required>
                <input type="email" placeholder="Your Email" required>
                <input type="tel" placeholder="Your Phone" required>
                <input type="date" placeholder="Travel Date" required>
                <textarea placeholder="Special Requests" rows="4"></textarea>
                <button type="submit">Submit Booking Request</button>
            </form>
        </div>
    `;

    document.getElementById('booking-form-modal').innerHTML = bookingForm;
    document.getElementById('booking-form-modal').style.display = 'block';
}

function closeBookingForm() {
    document.getElementById('booking-form-modal').style.display = 'none';
}
