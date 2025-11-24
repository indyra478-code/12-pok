<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Serena Scrunchie 12H</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700&family=Quicksand:wght@300;400;500;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        /* General Styles */
        :root {
            --soft-pink: #FFC0CB;
            --baby-pink: #F8BBD0;
            --dusty-rose: #E79B9B;
            --white: #FFFFFF;
            --gold: #FFD700;
            --rose-gold: #B76E79;
            --text-color: #555;
            --heading-color: #333;
            --primary-font: 'Playfair Display', serif;
            --secondary-font: 'Quicksand', sans-serif;
        }

        body {
            font-family: var(--secondary-font);
            color: var(--text-color);
            line-height: 1.6;
            margin: 0;
            background-color: var(--white);
        }

        .container {
            max-width: 1100px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Header */
        .header {
            background-color: var(--baby-pink);
            padding: 1rem 0;
            border-bottom: 2px solid var(--soft-pink);
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .header .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-family: var(--primary-font);
            font-weight: 700;
            font-size: 1.8rem;
            color: var(--dusty-rose);
            margin: 0;
        }

        .nav a {
            color: var(--white);
            text-decoration: none;
            font-weight: 500;
            margin-left: 20px;
            transition: color 0.3s ease;
        }

        .nav a:hover {
            color: var(--rose-gold);
        }
        
        .cart-icon {
            font-size: 1.5rem;
            color: var(--white);
            cursor: pointer;
            position: relative;
        }

        .cart-count {
            position: absolute;
            top: -8px;
            right: -8px;
            background-color: var(--dusty-rose);
            color: var(--white);
            font-size: 0.7rem;
            font-weight: bold;
            border-radius: 50%;
            padding: 2px 6px;
        }

        /* Buttons */
        .btn {
            display: inline-block;
            background-color: var(--soft-pink);
            color: var(--white);
            padding: 12px 25px;
            text-decoration: none;
            border-radius: 50px;
            font-weight: 500;
            transition: background-color 0.3s ease;
            border: none;
            cursor: pointer;
        }

        .btn:hover {
            background-color: var(--rose-gold);
        }

        .btn-secondary {
            background-color: transparent;
            border: 2px solid var(--soft-pink);
            color: var(--soft-pink);
        }

        .btn-secondary:hover {
            background-color: var(--soft-pink);
            color: var(--white);
        }
        
        .whatsapp-btn {
            background-color: #25D366;
            color: var(--white);
        }
        
        .whatsapp-btn:hover {
            background-color: #128C7E;
        }
        
        /* New DANA Button Style */
        .dana-btn {
            background-color: #1677FF; /* DANA blue color */
            color: var(--white);
            transition: background-color 0.3s ease;
        }

        .dana-btn:hover {
            background-color: #0d5fcc;
        }

        /* Sections */
        section {
            padding: 60px 0;
            text-align: center;
        }

        section h3 {
            font-family: var(--primary-font);
            font-size: 2.5rem;
            color: var(--heading-color);
            margin-bottom: 20px;
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(rgba(255, 192, 203, 0.7), rgba(255, 192, 203, 0.7)), url('https://t4.ftcdn.net/jpg/08/21/32/55/360_F_821325589_z501wyXQBlNvxYuuFA7gfU4nN8MlfF3L.jpg');
            background-size: cover;
            background-position: center;
            color: var(--white);
            padding: 100px 0;
        }

        .hero h2 {
            font-family: var(--primary-font);
            font-size: 3rem;
            margin-bottom: 10px;
        }

        .hero p {
            font-size: 1.2rem;
            margin-bottom: 30px;
        }

        /* Products Section */
        .products {
            background-color: #fce4ec;
        }
        
        .product-list {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 20px;
            margin-top: 30px;
        }

        .product-card {
            background-color: var(--white);
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
            transition: transform 0.3s ease;
            text-align: left;
        }

        .product-card:hover {
            transform: translateY(-5px);
        }

        .product-card img {
            width: 100%;
            height: 250px;
            object-fit: cover;
            display: block;
        }

        .product-content {
            padding: 20px;
        }

        .product-content h4 {
            font-family: var(--primary-font);
            font-weight: 700;
            color: var(--dusty-rose);
            margin: 0 0 10px;
        }

        .product-content p.price {
            font-weight: bold;
            color: var(--rose-gold);
            margin: 0 0 15px;
        }
        
        .product-content p.description {
            font-size: 0.9rem;
            color: #888;
            margin-bottom: 15px;
        }
        
        .product-colors {
            display: flex;
            gap: 10px;
            margin-bottom: 15px;
        }
        
        .color-swatch {
            width: 25px;
            height: 25px;
            border-radius: 50%;
            cursor: pointer;
            border: 2px solid transparent;
            transition: border-color 0.2s ease;
        }
        
        .color-swatch.selected {
            border-color: var(--dusty-rose);
            box-shadow: 0 0 5px rgba(0,0,0,0.2);
        }

        .product-content .btn {
            width: 100%;
            text-align: center;
        }
        
        .reviews {
            padding: 15px;
            background-color: #fefefe;
            border-top: 1px solid #eee;
            margin-top: 10px;
        }

        .reviews p {
            font-size: 0.8rem;
            font-style: italic;
            margin: 5px 0;
            color: #777;
        }

        /* About Section */
        .about {
            background-color: var(--white);
        }

        /* Contact Section */
        .contact {
            background-color: #fce4ec;
        }

        .contact-links {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-top: 20px;
        }

        /* Footer */
        .footer {
            background-color: var(--baby-pink);
            color: var(--white);
            text-align: center;
            padding: 20px 0;
        }

        /* Modal Styles */
        .modal {
            display: none;
            position: fixed;
            z-index: 1001;
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            overflow: auto;
            background-color: rgba(0,0,0,0.4);
            animation: fadeIn 0.3s;
        }

        .modal-content {
            background-color: var(--white);
            margin: 10% auto;
            padding: 20px;
            border-radius: 10px;
            width: 80%;
            max-width: 500px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.3);
            position: relative;
            animation: slideInTop 0.5s;
        }

        .close-btn {
            color: #aaa;
            float: right;
            font-size: 28px;
            font-weight: bold;
            cursor: pointer;
        }

        .close-btn:hover,
        .close-btn:focus {
            color: #000;
            text-decoration: none;
            cursor: pointer;
        }

        .cart-list {
            list-style: none;
            padding: 0;
        }

        .cart-item {
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 10px 0;
            border-bottom: 1px solid #eee;
        }

        .cart-item:last-child {
            border-bottom: none;
        }

        .cart-item-info {
            display: flex;
            align-items: center;
            gap: 15px;
        }

        .cart-item-info img {
            width: 60px;
            height: 60px;
            object-fit: cover;
            border-radius: 5px;
        }

        .cart-item-name {
            font-weight: 500;
        }
        
        .cart-item-price {
            color: var(--rose-gold);
            font-weight: bold;
        }
        
        .quantity-controls {
            display: flex;
            align-items: center;
            gap: 5px;
        }
        
        .quantity-controls button {
            background-color: var(--soft-pink);
            color: var(--white);
            border: none;
            width: 25px;
            height: 25px;
            border-radius: 50%;
            cursor: pointer;
        }
        
        .quantity-controls span {
            font-weight: bold;
            font-size: 1.1rem;
            min-width: 20px;
            text-align: center;
        }

        .checkout-btn {
            width: 100%;
            margin-top: 20px;
        }
        
        .payment-options {
            display: flex;
            flex-direction: column; /* Changed to column for better mobile layout */
            gap: 10px;
            margin-top: 20px;
        }
        
        .payment-options button {
            width: 100%;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        .payment-options button i {
            margin-right: 8px;
        }
        
        .quantity-modal .modal-content {
            padding: 30px;
            text-align: center;
        }
        
        .quantity-modal .modal-content h4 {
            margin-top: 0;
            color: var(--dusty-rose);
        }
        
        .quantity-modal .color-options {
            display: flex;
            justify-content: center;
            gap: 10px;
            margin: 15px 0;
        }
        
        .quantity-modal .color-swatch.active {
            border-color: var(--dusty-rose);
            box-shadow: 0 0 5px rgba(0,0,0,0.2);
        }

        .quantity-modal input[type="number"] {
            width: 80px;
            padding: 8px;
            border: 1px solid #ddd;
            border-radius: 5px;
            text-align: center;
            font-size: 1.1rem;
            margin: 15px 0;
        }
        
        .quantity-modal .modal-buttons {
            display: flex;
            justify-content: center;
            gap: 10px;
        }

        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        @keyframes slideInTop {
            from { transform: translateY(-50px); opacity: 0; }
            to { transform: translateY(0); opacity: 1; }
        }

        /* Loading Spinner */
        .loading-spinner {
            display: none;
            position: fixed;
            z-index: 2000;
            left: 50%;
            top: 50%;
            transform: translate(-50%, -50%);
            border: 4px solid #f3f3f3;
            border-top: 4px solid var(--soft-pink);
            border-radius: 50%;
            width: 40px;
            height: 40px;
            animation: spin 1s linear infinite;
        }
        
        .user-info {
            font-size: 0.8rem;
            color: #aaa;
            margin-top: 10px;
            text-align: center;
        }

        @keyframes spin {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }
        
        /* Responsive Design */
        @media (max-width: 768px) {
            .header .container {
                flex-direction: column;
                text-align: center;
            }
            .nav {
                margin-top: 15px;
            }
            .nav a {
                margin: 0 10px;
            }
            .hero h2 {
                font-size: 2rem;
            }
            .category-list {
                flex-direction: column;
                align-items: center;
            }
        }
    </style>
</head>
<body>

    

<div id="loading-spinner" class="loading-spinner"></div>

    

<header class="header">
        <div class="container">
            <h1 class="logo">Serena Scrunchie</h1>
            <nav class="nav">
                <a href="#home">Beranda</a>
                <a href="#products">Produk</a>
                <a href="#about">Tentang Kami</a>
            </nav>
            <div class="cart-icon" onclick="openCartModal()">
                <i class="fas fa-shopping-cart"></i>
                <span id="cart-count" class="cart-count">0</span>
            </div>
        </div>
    </header>

    

<section id="home" class="hero">
        <div class="container">
            <div class="hero-content">
                <h2>Lengkapi Gayamu dengan Scrunchie & Jedai Imut!</h2>
                <p>Koleksi aksesoris rambut lucu, girly, dan terjangkau untuk setiap gayamu.</p>
                <a href="#products" class="btn">Belanja Sekarang</a>
            </div>
        </div>
    </section>

    

<section id="products" class="products">
        <div class="container">
            <h3>Pilihan Koleksi Kami</h3>
            <div id="product-list" class="product-list">
                

</div>
        </div>
    </section>

    

<section id="about" class="about">
        <div class="container">
            <h3>Tentang Kami</h3>
            <p>Serena Scrunchie adalah brand aksesoris rambut imut dan girly yang lahir dari kreativitas tim kelas 12H SMAN 1 Dramaga.</p>
            <p><strong>Visi Kami:</strong> Menyebarkan kebahagiaan serta kepercayaan diri lewat scrunchie dan jedai yang lucu, aesthetic, serta terjangkau.</p>
            <a href="#" class="btn btn-secondary">Baca Selengkapnya</a>
        </div>
    </section>

    

<footer class="footer">
        <div class="container">
            <p>&copy; 2024 Serena Scrunchie. Semua Hak Cipta Dilindungi.</p>
        </div>
    </footer>

    

<div id="cartModal" class="modal">
        <div class="modal-content">
            <span class="close-btn" onclick="closeCartModal()">&times;</span>
            <h3>Keranjang Belanja</h3>
            <ul id="cart-items" class="cart-list">
                

</ul>
            <p><strong>Total: Rp<span id="cart-total">0</span></strong></p>
            <button class="btn checkout-btn" onclick="showCheckoutOptions()">Bayar Sekarang</button>
        </div>
    </div>
    
    

<div id="add-to-cart-modal" class="modal">
        <div class="modal-content">
            <span class="close-btn" onclick="closeAddToCartModal()">&times;</span>
            <h4 id="modal-product-name"></h4>
            
            <p style="margin-top:20px;">Pilih Warna:</p>
            <div id="modal-color-options" class="product-colors" style="justify-content: center;"></div>
            
            <p style="margin-top:20px;">Jumlah:</p>
            <input type="number" id="product-quantity" value="1" min="1" style="width: 80px; text-align: center;">
            
            <div class="modal-buttons" style="margin-top: 20px;">
                <button class="btn" onclick="confirmAddToCart()">Tambahkan</button>
                <button class="btn btn-secondary" onclick="closeAddToCartModal()">Batal</button>
            </div>
        </div>
    </div>
    
    

<div id="checkoutModal" class="modal">
        <div class="modal-content">
            <span class="close-btn" onclick="closeCheckoutModal()">&times;</span>
            <h3>Pembayaran</h3>
            <p>Total Pesanan: <strong>Rp<span id="checkout-total">0</span></strong></p> 
            <div id="payment-status-message" style="display: none; color: green; margin: 15px 0; font-weight: bold;"></div>
            <p style="margin-top: 20px; font-weight: 500;">Pilih Metode Pembayaran:</p>
            <div class="payment-options">
                <button class="btn dana-btn" onclick="payWithDana()">
                    <i class="fas fa-wallet"></i> Bayar dengan DANA (Otomatis)
                </button>
                <button class="btn whatsapp-btn" onclick="payWithWhatsapp()">
                    <i class="fab fa-whatsapp"></i> Bayar via WhatsApp (Manual)
                </button>
            </div>
        </div>
    </div>

    <script type="module">
        import { initializeApp } from "https://www.gstatic.com/firebasejs/11.6.1/firebase-app.js";
        import { getAuth, signInAnonymously, signInWithCustomToken, onAuthStateChanged } from "https://www.gstatic.com/firebasejs/11.6.1/firebase-auth.js";
        // NOTE: Added writeBatch and getDocs for cart clearing simulation
        import { getFirestore, doc, setDoc, onSnapshot, collection, updateDoc, increment, getDoc, deleteDoc, writeBatch, getDocs } from "https://www.gstatic.com/firebasejs/11.6.1/firebase-firestore.js";
        import { setLogLevel } from "https://www.gstatic.com/firebasejs/11.6.1/firebase-firestore.js";
        
        setLogLevel('debug');

        // Global variables provided by the platform
        const firebaseConfig = JSON.parse(typeof __firebase_config !== 'undefined' ? __firebase_config : '{}');
        const appId = typeof __app_id !== 'undefined' ? __app_id : 'default-app-id';
        const initialAuthToken = typeof __initial_auth_token !== 'undefined' ? __initial_auth_token : null;

        let db;
        let auth;
        let userId;
        let currentTotal = 0; // New: Variable to store the current cart total

        // UPDATED: Product Data
        const productData = [
            { id: 'jedai-kamboja', name: 'Jedai Kamboja Lucu', price: 5000, image: 'https://down-id.img.susercontent.com/file/id-11134207-7r98s-lv9jn6snlqh9c0', colors: [{ name: 'Pink', hex: '#FFC0CB' }, { name: 'Biru', hex: '#ADD8E6' }], reviews: ["Barang sudah sampai, bagus banget! Pengiriman cepat.", "Jedainya kokoh, warnanya cantik. Suka!"] },
            { id: 'scrunchie-silk', name: 'Scrunchie Silk', price: 3500, image: 'https://jadorehairsupplies.com.au/cdn/shop/files/2692adce-b98d-4925-963e-656f2a3e88c1.png?format=webp&v=1754436126&width=1000', colors: [{ name: 'Merah', hex: '#E79B9B' }, { name: 'Hitam', hex: '#000000' }], reviews: ["Lembut di rambut, tidak bikin pusing.", "Warna merahnya cantik banget, cocok buat OOTD."] },
            { id: 'jepit-hijab-hias', name: 'Jepit Hijab Hias', price: 5000, image: 'https://www.static-src.com/wcsstore/Indraprastha/images/catalog/full/catalog-image/103/MTA-182956216/no_brand_jepitan_rambut_bunga_-_aksesori_rambut_bunga_mewah_jepit_rambut_-_hair_clip_jepit_bunga_anggrek_full06_mgmv52yi.webp', colors: [{ name: 'Gold', hex: '#FFD700' }, { name: 'Silver', hex: '#C0C0C0' }], reviews: ["Jepitannya kuat, nggak gampang lepas.", "Barang sesuai deskripsi, recommended!"] }
        ];
        
        const productListEl = document.getElementById('product-list');
        const cartItemsEl = document.getElementById('cart-items');
        const cartCountEl = document.getElementById('cart-count');
        const cartTotalEl = document.getElementById('cart-total');
        const cartModalEl = document.getElementById('cartModal');
        const addToCartModalEl = document.getElementById('add-to-cart-modal');
        const checkoutModalEl = document.getElementById('checkoutModal');
        const modalProductNameEl = document.getElementById('modal-product-name');
        const modalColorOptionsEl = document.getElementById('modal-color-options');
        const productQuantityInput = document.getElementById('product-quantity');
        const loadingSpinner = document.getElementById('loading-spinner');
        // const userIdEl = document.getElementById('user-id'); // Removed
        const checkoutTotalEl = document.getElementById('checkout-total'); // New: Checkout total display
        const paymentStatusMessageEl = document.getElementById('payment-status-message'); // New: Payment status message

        
        let cartData = {};
        let selectedProduct = null;
        let selectedColor = null;

        // Function to show/hide loading spinner
        const showLoading = () => loadingSpinner.style.display = 'block';
        const hideLoading = () => loadingSpinner.style.display = 'none';

        // Function to render products
        function renderProducts() {
            productListEl.innerHTML = '';
            productData.forEach(product => {
                const card = document.createElement('div');
                card.className = 'product-card';
                card.innerHTML = `
                    <img src="${product.image}" alt="${product.name}">
                    <div class="product-content">
                        <h4>${product.name}</h4>
                        <p class="price">Rp${product.price.toLocaleString('id-ID')}</p>
                        <button class="btn" onclick="openAddToCartModal('${product.id}')">Tambah ke Keranjang</button>
                        <div class="reviews">
                            ${product.reviews.map(review => `<p>&#9733; "${review}"</p>`).join('')}
                        </div>
                    </div>
                `;
                productListEl.appendChild(card);
            });
        }
        
        // Function to render cart
        function renderCart() {
            cartItemsEl.innerHTML = '';
            let total = 0;
            let totalItems = 0;
            
            for (const productIdColor in cartData) {
                const item = cartData[productIdColor];
                const product = productData.find(p => p.id === productIdColor.split('_')[0]);
                if (product) {
                    const listItem = document.createElement('li');
                    listItem.className = 'cart-item';
                    const itemTotal = item.quantity * product.price;
                    total += itemTotal;
                    totalItems += item.quantity;
                    listItem.innerHTML = `
                        <div class="cart-item-info">
                            <img src="${product.image}" alt="${product.name}">
                            <div>
                                <span class="cart-item-name">${product.name}</span>
                                <p>Warna: ${item.color}</p>
                                <p class="cart-item-price">Rp${itemTotal.toLocaleString('id-ID')}</p>
                            </div>
                        </div>
                        <div class="quantity-controls">
                            <button onclick="updateQuantity('${productIdColor}', -1)">-</button>
                            <span>${item.quantity}</span>
                            <button onclick="updateQuantity('${productIdColor}', 1)">+</button>
                        </div>
                    `;
                    cartItemsEl.appendChild(listItem);
                }
            }

            currentTotal = total; // Store the total
            cartCountEl.textContent = totalItems;
            cartTotalEl.textContent = total.toLocaleString('id-ID');

            if (totalItems === 0) {
                cartItemsEl.innerHTML = '<li style="text-align:center;">Keranjang Anda kosong.</li>';
            }
        }
        
        // Function to update item quantity in Firestore
        async function updateQuantity(productIdColor, change) {
            const [productId, color] = productIdColor.split('_');
            const cartItemRef = doc(db, `/artifacts/${appId}/users/${userId}/cart_items`, productIdColor);
            
            try {
                const docSnap = await getDoc(cartItemRef);
                if (docSnap.exists()) {
                    const currentQuantity = docSnap.data().quantity;
                    const newQuantity = currentQuantity + change;
                    if (newQuantity > 0) {
                        await updateDoc(cartItemRef, { quantity: newQuantity });
                    } else {
                        await deleteDoc(cartItemRef);
                    }
                }
            } catch (error) {
                console.error("Gagal memperbarui jumlah produk:", error);
            }
        }

        // Modal functions
        function openAddToCartModal(productId) {
            selectedProduct = productData.find(p => p.id === productId);
            if (!selectedProduct) return;
            
            modalProductNameEl.textContent = selectedProduct.name;
            productQuantityInput.value = 1;
            selectedColor = selectedProduct.colors[0].name;
            
            modalColorOptionsEl.innerHTML = '';
            selectedProduct.colors.forEach(color => {
                const swatch = document.createElement('div');
                swatch.className = 'color-swatch';
                swatch.style.backgroundColor = color.hex;
                swatch.dataset.colorName = color.name;
                swatch.onclick = () => {
                    document.querySelectorAll('.color-swatch').forEach(s => s.classList.remove('active'));
                    swatch.classList.add('active');
                    selectedColor = color.name;
                };
                if (color.name === selectedColor) {
                    swatch.classList.add('active');
                }
                modalColorOptionsEl.appendChild(swatch);
            });
            
            addToCartModalEl.style.display = 'block';
        }

        function closeAddToCartModal() {
            addToCartModalEl.style.display = 'none';
        }
        
        async function confirmAddToCart() {
            const quantity = parseInt(productQuantityInput.value, 10);
            if (isNaN(quantity) || quantity <= 0 || !selectedProduct || !selectedColor) {
                console.error("Informasi produk tidak lengkap. Tidak dapat menambahkan ke keranjang.");
                return;
            }
            
            await addToCart(selectedProduct.id, selectedColor, quantity);
            closeAddToCartModal();
        }

        async function addToCart(productId, color, quantity) {
            if (!userId) {
                console.error("User ID is not available. Cannot add to cart.");
                return;
            }
            showLoading();
            const product = productData.find(p => p.id === productId);
            const docId = `${productId}_${color}`;
            const cartItemRef = doc(db, `/artifacts/${appId}/users/${userId}/cart_items`, docId);

            try {
                const docSnap = await getDoc(cartItemRef);
                if (docSnap.exists()) {
                    await updateDoc(cartItemRef, {
                        quantity: increment(quantity)
                    });
                } else {
                    await setDoc(cartItemRef, {
                        name: product.name,
                        price: product.price,
                        image: product.image,
                        color: color,
                        quantity: quantity
                    });
                }
                console.log("Produk berhasil ditambahkan ke keranjang!");
            } catch (error) {
                console.error("Gagal menambahkan produk ke keranjang:", error);
            }
            hideLoading();
        }

        function showCheckoutOptions() {
            if (Object.keys(cartData).length === 0) {
                return; // Do nothing if cart is empty
            }
            checkoutTotalEl.textContent = currentTotal.toLocaleString('id-ID'); // Update display
            paymentStatusMessageEl.style.display = 'none'; // Reset status
            closeCartModal();
            checkoutModalEl.style.display = 'block';
        }
        
        function closeCheckoutModal() {
            checkoutModalEl.style.display = 'none';
        }
        
        // New function to clear cart after successful payment simulation
        async function clearCartSimulation() {
             if (!userId || !db) return;
             const cartCollectionRef = collection(db, `/artifacts/${appId}/users/${userId}/cart_items`);
             try {
                const snapshot = await getDocs(cartCollectionRef);
                const batch = writeBatch(db);

                snapshot.docs.forEach(doc => {
                    batch.delete(doc.ref);
                });

                await batch.commit();
                console.log("Keranjang berhasil dikosongkan setelah pembayaran simulasi.");
             } catch (error) {
                 console.error("Gagal mengosongkan keranjang:", error);
             }
        }

        // UPDATED: payWithDana function for automatic payment simulation
        function payWithDana() {
            const total = currentTotal;
            
            // Show processing message
            paymentStatusMessageEl.style.display = 'block';
            paymentStatusMessageEl.style.color = '#1677FF';
            paymentStatusMessageEl.innerHTML = `<i class="fas fa-spinner fa-spin"></i> Meminta QR Code DANA untuk total Rp${total.toLocaleString('id-ID')}...`;

            // Simulation of DANA API call response time (3 seconds)
            setTimeout(async () => {
                
                // Show success message
                paymentStatusMessageEl.style.color = 'green';
                paymentStatusMessageEl.innerHTML = `<i class="fas fa-check-circle"></i> Pembayaran Rp${total.toLocaleString('id-ID')} berhasil (Simulasi)!`;
                
                // Simulate redirection/payment logic (open DANA link in new tab)
                window.open('https://www.dana.id/s/BayarMenggunakanDana', '_blank'); 
                
                // Clear cart data (simulating a successful transaction and order completion)
                await clearCartSimulation();

                // Close modal after redirection
                setTimeout(() => {
                    closeCheckoutModal();
                }, 2000);
                
            }, 3000);
        }

        function payWithWhatsapp() {
            let message = "Halo Serena Scrunchie!\n\nSaya ingin memesan produk berikut:\n\n";
            let total = 0;
            
            for (const productIdColor in cartData) {
                const item = cartData[productIdColor];
                const product = productData.find(p => p.id === productIdColor.split('_')[0]);
                if (product) {
                    const itemTotal = item.quantity * product.price;
                    total += itemTotal;
                    message += `- ${product.name} (${item.color}) - Jumlah: ${item.quantity} - Total: Rp${itemTotal.toLocaleString('id-ID')}\n`;
                }
            }
            
            message += `\nTotal Harga Keseluruhan: Rp${total.toLocaleString('id-ID')}\n\nMohon konfirmasi pesanan saya. Terima kasih!`;
            
            const whatsappUrl = `https://wa.me/628388581375?text=${encodeURIComponent(message)}`;
            window.open(whatsappUrl, '_blank');
        }

        // Modal functions
        function openCartModal() {
            cartModalEl.style.display = 'block';
        }

        function closeCartModal() {
            cartModalEl.style.display = 'none';
        }

        window.onclick = function(event) {
            if (event.target == cartModalEl) {
                closeCartModal();
            }
            if (event.target == addToCartModalEl) {
                closeAddToCartModal();
            }
            if (event.target == checkoutModalEl) {
                // Do not close checkoutModal if payment is processing
                if (paymentStatusMessageEl.style.display === 'none') {
                    closeCheckoutModal();
                }
            }
        }
        
        window.openAddToCartModal = openAddToCartModal;
        window.confirmAddToCart = confirmAddToCart;
        window.closeAddToCartModal = closeAddToCartModal;
        window.openCartModal = openCartModal;
        window.closeCartModal = closeCartModal;
        window.showCheckoutOptions = showCheckoutOptions;
        window.payWithDana = payWithDana;
        window.payWithWhatsapp = payWithWhatsapp;
        window.updateQuantity = updateQuantity;

        // Initialize Firebase and listen for auth state
        async function initFirebase() {
            showLoading();
            try {
                const app = initializeApp(firebaseConfig);
                db = getFirestore(app);
                auth = getAuth(app);
                
                onAuthStateChanged(auth, async (user) => {
                    if (user) {
                        userId = user.uid;
                    } else {
                        try {
                            if (initialAuthToken) {
                                const userCredential = await signInWithCustomToken(auth, initialAuthToken);
                                userId = userCredential.user.uid;
                            } else {
                                const userCredential = await signInAnonymously(auth);
                                userId = userCredential.user.uid;
                            }
                        } catch (error) {
                            console.error("Authentication failed:", error);
                            // Fallback to anonymous user if custom token fails
                            const userCredential = await signInAnonymously(auth);
                            userId = userCredential.user.uid;
                        }
                    }
                    
                    // userIdEl.textContent = userId; // Removed
                    renderProducts();
                    
                    // Set up real-time listener for cart
                    const cartRef = collection(db, `/artifacts/${appId}/users/${userId}/cart_items`);
                    onSnapshot(cartRef, (snapshot) => {
                        snapshot.docChanges().forEach((change) => {
                            const product = change.doc.data();
                            const productIdColor = change.doc.id;
                            if (change.type === "added" || change.type === "modified") {
                                cartData[productIdColor] = product;
                            }
                            if (change.type === "removed") {
                                delete cartData[productIdColor];
                            }
                        });
                        renderCart();
                        hideLoading();
                    });
                });
            } catch (error) {
                console.error("Firebase initialization failed:", error);
                hideLoading();
            }
        }

        window.onload = initFirebase;
    </script>
</body>
</html>
