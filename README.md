<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>BeautyGlow</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            background: linear-gradient(135deg, #d9ccff 50%, #fbcae0 50%);
            font-family: 'Arial', sans-serif;
            color: rgb(10, 1, 1);
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        header {
            width: 100%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 40px;
            background: rgba(230, 223, 223, 0.1);
            backdrop-filter: blur(10px);
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
            position: sticky;
            top: 0;
            z-index: 10;
        }
        .logo-text {
            text-shadow: 0 0 10px rgba(255, 255, 255, 0.8),
                0 0 20px rgba(255, 255, 255, 0.6),
                0 0 30px rgba(255, 255, 255, 0.4);
            font-size: 3rem;
            font-weight: bold;
            margin: 0;
        }
        .header-right {
            display: flex;
            align-items: center;
            gap: 20px;
        }
        .header-right img {
            width: 50px;
            height: 50px;
            border-radius: 50%;
        }
        .btn-add-cart {
            background: linear-gradient(135deg, #fff9db 0%, #facc15 100%);
            color: #333;
            padding: 12px 28px;
            border: none;
            border-radius: 30px;
            text-decoration: none;
            font-weight: 700;
            font-size: 1rem;
            box-shadow: 0 6px 15px rgba(250, 204, 21, 0.6);
            transition: background 0.3s ease, box-shadow 0.3s ease;
            cursor: pointer;
        }
        .btn-add-cart:hover {
            background: linear-gradient(135deg, #f2d665 0%, #fff9db 100%);
            box-shadow: 0 8px 25px rgba(255, 223, 0, 0.8);
        }
        .description {
            text-align: center;
            margin: 40px auto;
            max-width: 600px;
            line-height: 1.6;
            font-size: 1.2rem;
        }
        .products {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 24px;
            max-width: 1100px;
            width: 100%;
            padding: 0 20px 40px;
        }
        .product-card {
            background: rgba(255, 255, 255, 0.12);
            border-radius: 12px;
            padding: 20px;
            box-shadow: 0 6px 20px rgba(0, 0, 0, 0.3);
            text-align: center;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
        }
        .product-card:hover {
            transform: scale(1.07);
            box-shadow: 0 12px 30px rgba(0, 0, 0, 0.45);
        }
        .product-card img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            margin-bottom: 12px;
            border-radius: 12px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.25);
        }
        .product-images {
            display: flex;
            justify-content: space-between;
            gap: 12px;
            margin-bottom: 12px;
        }
        .product-images img {
            width: 48%;
            height: 150px;
            border-radius: 12px;
            object-fit: cover;
            box-shadow: 0 3px 8px rgba(0, 0, 0, 0.2);
        }
        .product-name {
            font-size: 1.35rem;
            font-weight: 700;
            margin: 12px 0 6px;
            color: #f9fafb;
        }
        .price {
            margin: 10px 0 18px;
            font-size: 1.15rem;
            font-weight: 700;
            color: #0f0f0f; 
        }
    
        .btn-product-cart {
            background: linear-gradient(135deg, #fff9db 0%, #facc15 100%);
            color: #333;
            padding: 12px 26px;
            border: none;
            border-radius: 28px;
            cursor: pointer;
            font-weight: 700;
            font-size: 1.05rem;
            box-shadow: 0 6px 18px rgba(250, 204, 21, 0.7);
            transition: background 0.3s ease, box-shadow 0.3s ease;
            align-self: center;
            width: 85%;
            user-select: none;
        }
        .btn-product-cart:hover {
            background: linear-gradient(135deg, #facc15 0%, #fff9db 100%);
            box-shadow: 0 8px 28px rgba(255, 223, 0, 0.85);
        }
    </style>
</head>
<body>
    <header>
        <h1 class="logo-text">BeautyGlow</h1>
        <div class="header-right">
            <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/5eb38977-bb6c-4a99-8a72-b6ceca70411b.png" alt="Elegant logo in purple and dark pink depicting abstract beauty symbols like flower petals and a glowing gem representing premium cosmetics brand" onerror="this.style.display='none';" />
            <a href="#" class="btn-add-cart">Add to Cart</a>
            <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/c56c47f9-008e-4d62-a7c5-98693d11da0e.png" alt="Account icon in dark pink and purple showing a silhouette of a smiling face with a heart above it symbolizing user profile for beauty enthusiasts" onerror="this.style.display='none';" />
        </div>
    </header>
    <section class="description">
        <p>Welcome to BeautyGlow – Elevate your beauty routine with luxurious, affordable products designed to bring out your natural radiance.</p>
    </section>
    <section class="products">
        
        <div class="product-card">
            <div class="product-images">
                <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/c57fc50f-c2ef-4bc7-927c-7be8f70a9973.png" alt="Premium foundation bottle in sleek design with purple and dark pink label, containing moisturizing formula for flawless coverage on all skin types" onerror="this.style.display='none';" />
                <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/4c02f01d-c9c0-49a7-8c54-b200bf8de147.png" alt="Attractive young woman with radiant skin holding a foundation bottle in hand, smiling softly in a brightly lit makeup studio" onerror="this.style.display='none';" />
            </div>
            <h3 class="product-name">Silk Foundation</h3>
            <p class="price">Price: INR 1500</p>
            <button class="btn-product-cart">Add to Cart</button>
        </div>
       
        <div class="product-card">
            <div class="product-images">
                <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/696bcfe2-bfff-41a2-afa9-f15ecf8b576b.png" alt="Chic lipstick set with six vibrant shades in gloss and matte finishes packed in an elegant purple case for bold lip looks" onerror="this.style.display='none';" />
                <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/b1c751d3-a566-477d-bce5-4195bad9dc7e.png" alt="Stylish girl applying lipstick in front of a mirror, showcasing deep red shade with perfect lips in a cozy beauty setup" onerror="this.style.display='none';" />
            </div>
            <h3 class="product-name">Vivid Lipstick Set</h3>
            <p class="price">Price: INR 1200</p>
            <button class="btn-product-cart">Add to Cart</button>
        </div>
        
        <div class="product-card">
            <div class="product-images">
                <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/42fe1c31-9878-4cde-8ec7-879f9b8b288f.png" alt="Volumizing mascara tube with curved brush in dark pink packaging designed for long, thick lashes with gentle formula" onerror="this.style.display='none';" />
                <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/e76b7ad2-0f42-4ca4-84eb-a406ace75d0a.png" alt="Gorgeous model with big beautiful eyes demonstrating mascara by holding the wand near her lashes in soft studio lighting" onerror="this.style.display='none';" />
            </div>
            <h3 class="product-name">Lash Lux Mascara</h3>
            <p class="price">Price: INR 800</p>
            <button class="btn-product-cart">Add to Cart</button>
        </div>
      
        <div class="product-card">
            <div class="product-images">
                <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/5c401aab-d179-4c3f-9ca0-12e064f96bae.png" alt="Glowing highlighter powder compact in shimmery pink tone perfect for highlighting cheeks, nose, and eyelids for luminous skin" onerror="this.style.display='none';" />
                <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/a3e59e59-7a51-41b0-a8eb-72f3bc6dcce6.png" alt="Charming woman with highlighter applied on face contours holding the compact in hand with joyful expression in pastel room" onerror="this.style.display='none';" />
            </div>
            <h3 class="product-name">Glow Beam Highlighter</h3>
            <p class="price">Price: INR 950</p>
            <button class="btn-product-cart">Add to Cart</button>
        </div>
      
        <div class="product-card">
            <div class="product-images">
                <img src="https://images.unsplash.com/photo-1501004318641-b39e6451bec6?auto=format&fit=crop&w=400&q=80" alt="Luxurious face serum bottle with dropper in purple and pink gradient packaging for glowing skin" />
                <img src="https://images.unsplash.com/photo-1522335789203-aabd1fc54bc9?auto=format&fit=crop&w=400&q=80" alt="Woman applying face serum with glowing skin and soft smile in natural light" />
            </div>
            <h3 class="product-name">Radiance Face Serum</h3>
            <p class="price">Price: INR 1800</p>
            <button class="btn-product-cart">Add to Cart</button>
        </div>
        
        <div class="product-card">
            <div class="product-images">
                <img src="https://images.unsplash.com/photo-1512436991641-6745cdb1723f?auto=format&fit=crop&w=400&q=80" alt="Elegant body lotion bottle with purple and pink floral design for smooth and hydrated skin" />
                <img src="https://images.unsplash.com/photo-1508214751196-bcfd4ca60f91?auto=format&fit=crop&w=400&q=80" alt="Happy woman applying body lotion on arm in cozy room with natural sunlight" />
            </div>
            <h3 class="product-name">Silky Body Lotion</h3>
            <p class="price">Price: INR 1100</p>
            <button class="btn-product-cart">Add to Cart</button>
        </div>
    
        <div class="product-card">
            <div class="product-images">
                <img src="https://images.unsplash.com/photo-1515378791036-0648a3ef77b2?auto=format&fit=crop&w=400&q=80" alt="Refreshing facial mist bottle with purple and pink ombre design for instant hydration" />
                <img src="https://images.unsplash.com/photo-1517841905240-472988babdf9?auto=format&fit=crop&w=400&q=80" alt="Woman spraying facial mist on face, looking refreshed and glowing" />
            </div>
            <h3 class="product-name">Hydra Mist Spray</h3>
            <p class="price">Price: INR 700</p>
            <button class="btn-product-cart">Add to Cart</button>
        </div>
       
        <div class="product-card">
            <div class="product-images">
                <img src="https://images.unsplash.com/photo-1464983953574-0892a716854b?auto=format&fit=crop&w=400&q=80" alt="Nourishing night cream jar in purple and pink packaging for deep skin repair" />
                <img src="https://images.unsplash.com/photo-1519125323398-675f0ddb6308?auto=format&fit=crop&w=400&q=80" alt="Woman applying night cream before sleep, smiling with healthy skin" />
            </div>
            <h3 class="product-name">Night Repair Cream</h3>
            <p class="price">Price: INR 1600</p>
            <button class="btn-product-cart">Add to Cart</button>
        </div>
    </section>
</body>
</html>
