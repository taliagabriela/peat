# peat
    <div class="tabs">
        <div class="tab active" data-tab="dashboard">Dashboard</div>
        <div class="tab" data-tab="food-log">Food Log</div>
        <div class="tab" data-tab="recommendations">Recommendations</div>
    </div>

    <div id="dashboard" class="tab-content active">
        <h2>Today's Nutrition</h2>
        
        <h3>Macronutrients</h3>
        <div class="nutrient-group">
            <div class="nutrient-label">
                <span>Protein</span>
                <span>45g / 100g</span>
            </div>
            <div class="nutrient-bar">
                <div class="nutrient-progress" style="width: 45%"></div>
            </div>
        </div>

        <div class="nutrient-group">
            <div class="nutrient-label">
                <span>Carbohydrates</span>
                <span>180g / 300g</span>
            </div>
            <div class="nutrient-bar">
                <div class="nutrient-progress" style="width: 60%"></div>
            </div>
        </div>

        <div class="nutrient-group">
            <div class="nutrient-label">
                <span>Fat</span>
                <span>50g / 80g</span>
            </div>
            <div class="nutrient-bar">
                <div class="nutrient-progress" style="width: 62.5%"></div>
            </div>
        </div>

        <h3>Ray Peat Specific Nutrients</h3>
        <div class="nutrient-group">
            <div class="nutrient-label">
                <span>Calcium</span>
                <span>600mg / 1200mg</span>
            </div>
            <div class="nutrient-bar">
                <div class="nutrient-progress" style="width: 50%"></div>
            </div>
        </div>

        <div class="nutrient-group">
            <div class="nutrient-label">
                <span>Magnesium</span>
                <span>150mg / 400mg</span>
            </div>
            <div class="nutrient-bar">
                <div class="nutrient-progress" style="width: 37.5%"></div>
            </div>
        </div>

        <div class="nutrient-group">
            <div class="nutrient-label">
                <span>Potassium</span>
                <span>2000mg / 4700mg</span>
            </div>
            <div class="nutrient-bar">
                <div class="nutrient-progress" style="width: 42.5%"></div>
            </div>
        </div>

        <div class="nutrient-group">
            <div class="nutrient-label">
                <span>Vitamin A</span>
                <span>3000IU / 10000IU</span>
            </div>
            <div class="nutrient-bar">
                <div class="nutrient-progress" style="width: 30%"></div>
            </div>
        </div>

        <div class="nutrient-group">
            <div class="nutrient-label">
                <span>Vitamin D</span>
                <span>400IU / 2000IU</span>
            </div>
            <div class="nutrient-bar">
                <div class="nutrient-progress" style="width: 20%"></div>
            </div>
        </div>
    </div>

    <div id="food-log" class="tab-content">
        <h2>Today's Food Log</h2>
        
        <div class="food-items">
            <div class="food-item">
                <span>Orange Juice (1 cup)</span>
                <div>
                    <span>112 calories</span>
                    <button class="remove-btn">Remove</button>
                </div>
            </div>
            <div class="food-item">
                <span>Whole Milk (1 cup)</span>
                <div>
                    <span>150 calories</span>
                    <button class="remove-btn">Remove</button>
                </div>
            </div>
            <div class="food-item">
                <span>Cottage Cheese (1/2 cup)</span>
                <div>
                    <span>110 calories</span>
                    <button class="remove-btn">Remove</button>
                </div>
            </div>
            <div class="food-item">
                <span>Eggs (2 large)</span>
                <div>
                    <span>140 calories</span>
                    <button class="remove-btn">Remove</button>
                </div>
            </div>
        </div>

        <div class="food-add">
            <h3>Add Food</h3>
            <select id="food-select">
                <option value="">Select a food...</option>
                <option value="orange-juice">Orange Juice</option>
                <option value="milk">Whole Milk</option>
                <option value="cottage-cheese">Cottage Cheese</option>
                <option value="eggs">Eggs</option>
                <option value="gelatin">Gelatin</option>
                <option value="honey">Honey</option>
                <option value="white-sugar">White Sugar</option>
                <option value="potato">Potato</option>
                <option value="beef">Beef</option>
                <option value="shellfish">Shellfish</option>
            </select>
            <input type="text" id="amount" placeholder="Amount">
            <button id="add-food-btn">Add</button>
        </div>
    </div>

    <div id="recommendations" class="tab-content">
        <h2>Ray Peat Dietary Recommendations</h2>
        
        <div class="recommendations">
            <p>Ray Peat's dietary approach focuses on supporting metabolism and thyroid function while reducing stress hormones and inflammation.</p>
            
            <div class="good-list">
                <h3>Recommended Foods</h3>
                <ul>
                    <li>Dairy (milk, cheese, cottage cheese)</li>
                    <li>Eggs</li>
                    <li>Orange juice</li>
                    <li>Ripe fruits</li>
                    <li>Honey and white sugar</li>
                    <li>Gelatin</li>
                    <li>Shellfish</li>
                    <li>Liver</li>
                    <li>Cooked mushrooms</li>
                    <li>Cooked carrots</li>
                    <li>White potatoes</li>
                </ul>
            </div>
            
            <div class="avoid-list">
                <h3>Foods to Limit or Avoid</h3>
                <ul>
                    <li>Polyunsaturated fats (vegetable oils)</li>
                    <li>Raw cruciferous vegetables</li>
                    <li>Nuts and seeds</li>
                    <li>Whole grains and brown rice</li>
                    <li>Beans and legumes</li>
                    <li>Lean meats</li>
                    <li>Artificial sweeteners</li>
                </ul>
            </div>
            
            <div class="meal-ideas">
                <h3>Meal Ideas</h3>
                <p><strong>Breakfast:</strong> Orange juice with gelatin, eggs, and milk</p>
                <p><strong>Lunch:</strong> Cottage cheese with fruit and honey</p>
                <p><strong>Dinner:</strong> Shellfish with potatoes and butter</p>
                <p><strong>Snack:</strong> Milk with sugar or honey</p>
            </div>
        </div>
    </div>
</div>

<script>
    document.addEventListener('DOMContentLoaded', function() {
        // Tab switching
        const tabs = document.querySelectorAll('.tab');
        tabs.forEach(tab => {
            tab.addEventListener('click', function() {
                // Remove active class from all tabs
                tabs.forEach(t => t.classList.remove('active'));
                // Add active class to clicked tab
                this.classList.add('active');
                
                // Hide all tab content
                const tabContents = document.querySelectorAll('.tab-content');
                tabContents.forEach(content => content.classList.remove('active'));
                
                // Show the selected tab content
                const tabId = this.getAttribute('data-tab');
                document.getElementById(tabId).classList.add('active');
            });
        });
        
        // Add food functionality
        document.getElementById('add-food-btn').addEventListener('click', function() {
            const foodSelect = document.getElementById('food-select');
            const amount = document.getElementById('amount').value;
            
            if (foodSelect.value && amount) {
                const foodName = foodSelect.options[foodSelect.selectedIndex].text;
                const foodItems = document.querySelector('.food-items');
                
                const foodItem = document.createElement('div');
                foodItem.className = 'food-item';
                
                const nameSpan = document.createElement('span');
                nameSpan.textContent = `${foodName} (${amount})`;
                
                const detailsDiv = document.createElement('div');
                
                const caloriesSpan = document.createElement('span');
                caloriesSpan.textContent = 'Added calories';
                
                const removeBtn = document.createElement('button');
                removeBtn.className = 'remove-btn';
                removeBtn.textContent = 'Remove';
                removeBtn.addEventListener('click', function() {
                    foodItem.remove();
                });
                
                detailsDiv.appendChild(caloriesSpan);
                detailsDiv.appendChild(removeBtn);
                
                foodItem.appendChild(nameSpan);
                foodItem.appendChild(detailsDiv);
                
                foodItems.appendChild(foodItem);
                
                // Reset inputs
                foodSelect.value = '';
                document.getElementById('amount').value = '';
            }
        });
        
        // Remove food functionality
        document.querySelectorAll('.remove-btn').forEach(btn => {
            btn.addEventListener('click', function() {
                this.closest('.food-item').remove();
            });
        });
        
        // Save data
        document.getElementById('save-btn').addEventListener('click', function() {
            alert('Your nutrition data has been saved!');
        });
    });
</script>
