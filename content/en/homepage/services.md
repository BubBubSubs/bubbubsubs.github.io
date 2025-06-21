---
title: "MENU"
header_menu_title: "MENU"
navigation_menu_title: "MENU"
weight: 2
header_menu: true
---

<html>
    <style>
    .tabs {
        display: flex;
        flex-wrap: nowrap;
        border-bottom: 2px solid #ccc;
        margin-bottom: 20px;
        width: 100%;
        /* Remove overflow-x: auto for no scroll bar */
    }
    .tab {
        flex: 1 1 0;                /* Allow tabs to shrink and grow equally */
        min-width: 0;                /* Allow shrinking below content size */
        padding: 8px 8px;            /* Smaller padding for small screens */
        cursor: pointer;
        border: none;
        background: none;
        font-size: clamp(12px, 2vw, 20px); /* Responsive font size */
        outline: none;
        /* white-space: nowrap;
        text-overflow: ellipsis;
        overflow: hidden; */
    }
    .tab.active {
        border-bottom: 3px solid rgb(184, 217, 0);        white-space: nowrap;
        text-overflow: ellipsis;
        overflow: hidden;
        font-weight: bold;
        color: rgb(227, 227, 228);
    }
    @media (max-width: 600px) {
    .tab {
        padding: 6px 2px;
        font-size: clamp(10px, 4vw, 16px);
        .menu-section { display: none; }
        .menu-section.active { display: block; }
        .menu-item { margin-bottom: 15px; }
        .item-name { font-weight: bold; }
        .item-desc { color:rgb(240, 211, 166) ; margin-left: 10px; }
        .item-price { float: right; color:rgb(69, 74, 78); }
    }
        }
        /* .tabs { display: flex; flex-wrap: nowrap; border-bottom: 2px solid #ccc; margin-bottom: 20px; width: 100%; }
        .tab {
            flex: 0 0 auto;
            padding: 10px 30px;
            cursor: pointer;
            border: none;
            background: none;
            /* font-size: 18px; */
            /* font-size: rem;
            outline: none;
            white-space: nowrap;    
                    }
        .tab.active {
            border-bottom: 3px solidrgb(184, 217, 0);
            font-weight: bold;
            color:rgb(227, 227, 228);
        }  */
        .menu-section { display: none; }
        .menu-section.active { display: block; }
        .menu-item { margin-bottom: 15px; }
        .item-name { font-weight: bold; }
        .item-desc { color:rgb(240, 211, 166) ; margin-left: 10px; }
        .item-price { float: right; color:rgb(69, 74, 78); }
    </style>
    <div class="tabs">
        <button class="tab" data-section="breakfast" onclick="showMenu('breakfast')">Breakfast</button>
        <button class="tab active" data-section="subs" onclick="showMenu('subs')">Subs n' More</button>
        <button class="tab" data-section="grill" onclick="showMenu('grill')">From The Grill</button>
        <button class="tab" data-section="salads" onclick="showMenu('salads')">Salads</button>
        <button class="tab" data-section="wraps" onclick="showMenu('wraps')">Wraps</button>
    </div>
    <div class="post-after" style=""></div>
    <div id="breakfast" class="menu-section">
        <div class="menu-item">
            <span class="item-name">Pancake Stack</span>
            <!-- <span class="item-price">$7.99</span><br> -->
            <span class="item-desc">Fluffy pancakes served with syrup and butter.</span>
        </div>
        <div class="menu-item">
            <span class="item-name">Biscuits with Gravy</span>
            <!-- <span class="item-price">$5.49</span><br> -->
            <span class="item-desc">One or two biscuit smothered in gravy.</span>
        </div>
        <div class="menu-item">
            <span class="item-name">Sausage Biscuit</span>
            <!-- <span class="item-price">$8.99</span><br> -->
            <span class="item-desc">Add egg & cheese for an additional cost.</span>
        </div>
        <div class="menu-item">
            <span class="item-name">Bacon Biscuit</span>
            <!-- <span class="item-price">$8.99</span><br> -->
            <span class="item-desc">Add egg & cheese for an additional cost.</span>
        </div>
        <div class="menu-item">
            <span class="item-name">Breakfast Wrap</span>
            <!-- <span class="item-price">$8.99</span><br> -->
            <span class="item-desc">Eggs, cheese, and your choice of sausage or bacon in a tortilla.</span>
        </div>
        <div class="menu-item">
            <span class="item-name">Bagel with Bacon or Sausage</span>
            <!-- <span class="item-price">$8.99</span><br> -->
            <span class="item-desc">Add egg & cheese for an additional cost.</span>
        </div>
                <div class="menu-item">
            <span class="item-name">Bagel with cream cheese</span>
            <!-- <span class="item-price">$8.99</span><br> -->
            <span class="item-desc">Add egg & cheese for an additional cost.</span>
        </div>
                <div class="menu-item">
            <span class="item-name">BLT</span>
            <!-- <span class="item-price">$8.99</span><br> -->
            <span class="item-desc">Bacon, lettuce, and tomato served on bread. A classic!</span>
        </div>
                <div class="menu-item">
            <span class="item-name">Fried Bologna</span>
            <!-- <span class="item-price">$8.99</span><br> -->
            <span class="item-desc">A southern favorite.</span>
        </div>
                <div class="menu-item">
            <span class="item-name">Sausage Sandwich</span>
            <!-- <span class="item-price">$8.99</span><br> -->
            <span class="item-desc">Add egg and cheese for an additional cost.</span>
        </div>
                <div class="menu-item">
            <span class="item-name">Breakfast Platter</span>
            <!-- <span class="item-price">$8.99</span><br> -->
            <span class="item-desc">More than what meets the eye.</span>
        </div>
                <div class="menu-item">
            <span class="item-name">Kid's Platter</span>
            <!-- <span class="item-price">$8.99</span><br> -->
            <span class="item-desc">More than what meets the eye.</span>
        </div>
    </div>
    <div id="subs" class="menu-section active">
        <div class="menu-item">
            <span class="item-name">Ham and Cheese</span>
            <!-- <span class="item-price">$9.49</span><br> -->
            <span class="item-desc">Ham, cheese, lettuce, tomato, onion, and mayo.</span>
        </div>
        <div class="menu-item">
            <span class="item-name">Italian Sub</span>
            <!-- <span class="item-price">$9.49</span><br> -->
            <span class="item-desc">Ham, salami, pepperoni, provolone, lettuce, tomato, onion, and Italian dressing.</span>
        </div>
        <div class="menu-item">
            <span class="item-name">Turkey & Cheese</span>
            <!-- <span class="item-price">$8.99</span><br> -->
            <span class="item-desc">Sliced turkey breast, cheese, lettuce, tomato, and mayo.</span>
        </div>
        <div class="menu-item">
            <span class="item-name">Veggie Delight</span>
            <!-- <span class="item-price">$7.99</span><br> -->
            <span class="item-desc">Lettuce, tomato, cucumber, green peppers, onions, and provolone cheese.</span>
        </div>
        <div class="menu-item">
            <span class="item-name">Tuna Salad</span>
            <!-- <span class="item-price">$7.99</span><br> -->
            <span class="item-desc">With your choice of toppings.</span>
        </div>
        <div class="menu-item">
            <span class="item-name">Chicken Salad</span>
            <!-- <span class="item-price">$7.99</span><br> -->
            <span class="item-desc">Add toppings of your choice.</span>
        </div>
        <div class="menu-item">
            <span class="item-name">BLT Sandwich</span>
            <!-- <span class="item-price">$7.99</span><br> -->
            <span class="item-desc">Bacon, lettuce, tomato, all in a sandwich.</span>
        </div>
        <div class="menu-item">
            <span class="item-name">Lynn's Sloppy Joe</span>
            <!-- <span class="item-price">$7.99</span><br> -->
            <span class="item-desc">Classic sloppy joe, Lynn-style.</span>
        </div>
        <div class="menu-item">
            <span class="item-name">Lynn All The Way</span>
            <!-- <span class="item-price">$7.99</span><br> -->
            <span class="item-desc">With mac n' cheese & Cole Slaw.</span>
        </div>
        <div class="menu-item">
            <span class="item-name">Meatball Sub</span>
            <!-- <span class="item-price">$7.99</span><br> -->
            <span class="item-desc">Meatballs smothered in marinara, topped with mozzerella cheese.</span>
        </div>
        <div class="menu-item">
            <span class="item-name">Walking Taco</span>
            <!-- <span class="item-price">$7.99</span><br> -->
            <span class="item-desc">A SVU favorite.</span>
        </div>
        <div class="menu-item">
            <span class="item-name">Classic Club</span>
            <!-- <span class="item-price">$7.99</span><br> -->
            <span class="item-desc">The classic chicken with lettuce under bread.</span>
        </div>
        <div class="menu-item">
            <span class="item-name">Turkey Club</span>
            <!-- <span class="item-price">$7.99</span><br> -->
            <span class="item-desc">We'd call it a tlub but it just doesn't sound as good as a "club."</span>
        </div>
        </div>
        <div id="grill" class="menu-section">
        <div class="menu-item">
            <span class="item-name">Philly Cheesesteak</span>
            <!-- <span class="item-price">$9.49</span><br> -->
            <span class="item-desc">Shaved steak, peppers, onions, and mushrooms served smothered in provolone cheese.</span>
        </div>
        <div class="menu-item">
            <span class="item-name">Chicken Philly</span>
            <!-- <span class="item-price">$8.99</span><br> -->
            <span class="item-desc">Same as the regular philly with chicken instead of steak.</span>
        </div>
        <div class="menu-item">
            <span class="item-name">Chicken Cordon Bleu</span>
            <!-- <span class="item-price">$7.99</span><br> -->
            <span class="item-desc">Marinated chicken, ham, and swiss cheese.</span>
        </div>
        <div class="menu-item">
            <span class="item-name">Plain Hotdog</span>
            <!-- <span class="item-price">$7.99</span><br> -->
            <span class="item-desc">Hotdog on a bun.</span>
        </div>
        <div class="menu-item">
            <span class="item-name">Dirty Dog</span>
            <!-- <span class="item-price">$7.99</span><br> -->
            <span class="item-desc">Hotdog served dirty.</span>
        </div>
        <div class="menu-item">
            <span class="item-name">Fried Bologna</span>
            <!-- <span class="item-price">$7.99</span><br> -->
            <span class="item-desc">A southern favorite.</span>
        </div>
        <div class="menu-item">
            <span class="item-name">Grilled Cheese</span>
            <!-- <span class="item-price">$7.99</span><br> -->
            <span class="item-desc">With your choice of cheese.</span>
        </div>
        <div class="menu-item">
            <span class="item-name">Chicken Quesadilla</span>
            <!-- <span class="item-price">$7.99</span><br> -->
            <span class="item-desc">Chicken and cheese pressed flat in a folded tortilla.</span>
        </div>
        <div class="menu-item">
            <span class="item-name">Cheese Quesadilla</span>
            <!-- <span class="item-price">$7.99</span><br> -->
            <span class="item-desc">Just cheese pressed flat on the grill in a folded tortilla.</span>
        </div>
        <div class="menu-item">
            <span class="item-name">Reuben</span>
            <!-- <span class="item-price">$7.99</span><br> -->
            <span class="item-desc">Marinated chicken, ham, and swiss cheese.</span>
        </div>
        <div class="menu-item">
            <span class="item-name">Reuben Large Sub</span>
            <!-- <span class="item-price">$7.99</span><br> -->
            <span class="item-desc">Corned beef, swiss cheese, and sauerkraut served on a whole hoagie.</span>
        </div>
        <div class="menu-item">
            <span class="item-name">Spikeon Sandwich</span>
            <!-- <span class="item-price">$7.99</span><br> -->
            <span class="item-desc">Grilled cheese with chicken, jalapenos, mushrooms, and onion.</span>
        </div>
        </div>
        <div id="salads" class="menu-section">
        <div class="menu-item">
            <span class="item-name">Italian Salad</span>
            <!-- <span class="item-price">$9.49</span><br> -->
            <span class="item-desc">Ham, salami, pepperoni, provolone, lettuce, tomato, onion, and Italian dressing.</span>
        </div>
        <div class="menu-item">
            <span class="item-name">Chef Salad</span>
            <!-- <span class="item-price">$7.99</span><br> -->
            <span class="item-desc">Lettuce, tomato, cucumber, green peppers, onions, and provolone cheese.</span>
        </div>
        <div class="menu-item">
            <span class="item-name">Caesar Salad</span>
            <!-- <span class="item-price">$8.99</span><br> -->
            <span class="item-desc">Add chicken for an additional cost.</span>
        </div>
        <div class="menu-item">
            <span class="item-name">Garden Salad</span>
            <!-- <span class="item-price">$7.99</span><br> -->
            <span class="item-desc">Lettuce, tomato, cucumber, green peppers, onions, and provolone cheese.</span>
        </div>
        </div>
        <div id="wraps" class="menu-section">
        <div class="menu-item">
            <span class="item-name">Buffalo Wrap</span>
            <!-- <span class="item-price">$9.49</span><br> -->
            <span class="item-desc">Ham, salami, pepperoni, provolone, lettuce, tomato, onion, and Italian dressing.</span>
        </div>
        <div class="menu-item">
            <span class="item-name">Chicken Caesar Wrap</span>
            <!-- <span class="item-price">$8.99</span><br> -->
            <span class="item-desc">Sliced turkey breast, Swiss cheese, lettuce, tomato, and mayo.</span>
        </div>
        <div class="menu-item">
            <span class="item-name">Veggie Wrap</span>
            <!-- <span class="item-price">$7.99</span><br> -->
            <span class="item-desc">Lettuce, tomato, cucumber, green peppers, onions, and provolone cheese.</span>
        </div>
        <div class="menu-item">
            <span class="item-name">Club Wrap</span>
            <!-- <span class="item-price">$7.99</span><br> -->
            <span class="item-desc">Lettuce, tomato, cucumber, green peppers, onions, and provolone cheese.</span>
        </div>
    </div>
    </div>
    <script>
    function showMenu(section) {
        document.querySelectorAll('.menu-section').forEach(function(el) {
            el.classList.remove('active');
        });
        document.getElementById(section).classList.add('active');
        document.querySelectorAll('.tab').forEach(function(tab) {
            tab.classList.toggle('active', tab.getAttribute('data-section') === section);
        });
    }
</script>
</html>