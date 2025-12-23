# Student-registration-form
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Student Registration Form</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

<div class="container">
    <h2>Student Registration Form</h2>

    <form>
        <div class="row">
            <input type="text" placeholder="First Name" required>
            <input type="text" placeholder="Last Name" required>
        </div>

        <div class="row">
            <input type="email" placeholder="Email" required>
            <input type="text" placeholder="Mobile Number" required>
        </div>

        <div class="row">
            <select>
                <option>Date</option>
            </select>
            <select>
                <option>Month</option>
            </select>
            <select>
                <option>Year</option>
            </select>
        </div>

        <div class="row gender">
            <label><input type="radio" name="gender"> Male</label>
            <label><input type="radio" name="gender"> Female</label>
        </div>

        <textarea placeholder="Address"></textarea>

        <div class="row">
            <input type="text" placeholder="City">
            <input type="text" placeholder="Pin Code">
            <input type="text" placeholder="State">
        </div>

        <select>
            <option>Select Country</option>
            <option>India</option>
            <option>USA</option>
            <option>UK</option>
        </select>

        <h3>Hobbies</h3>
        <div class="row hobbies">
            <label><input type="checkbox"> Drawing</label>
            <label><input type="checkbox"> Singing</label>
            <label><input type="checkbox"> Dancing</label>
            <label><input type="checkbox"> Sports</label>
        </div>

        <div class="buttons">
            <button type="reset" class="reset">Reset</button>
            <button type="submit" class="submit">Submit</button>
        </div>
    </form>
</div>

</body>
</html>


body {
    margin: 0;
    padding: 0;
    font-family: Arial, sans-serif;
    background: linear-gradient(to right, #8360c3, #2ebf91);
}

.container {
    width: 70%;
    margin: 40px auto;
    background: #ffffff;
    padding: 25px;
    border-radius: 12px;
    box-shadow: 0 0 15px rgba(0,0,0,0.2);
}

h2 {
    text-align: center;
    background: #6f42c1;
    color: white;
    padding: 12px;
    border-radius: 8px;
}

.row {
    display: flex;
    gap: 10px;
    margin-bottom: 12px;
}

input, select, textarea {
    width: 100%;
    padding: 8px;
    border: 1px solid #ccc;
    border-radius: 6px;
}

textarea {
    resize: none;
    height: 70px;
}

.gender label,
.hobbies label {
    margin-right: 15px;
}

h3 {
    color: #6f42c1;
    margin-top: 15px;
}

.buttons {
    text-align: right;
    margin-top: 15px;
}

button {
    padding: 8px 18px;
    border: none;
    border-radius: 6px;
    color: white;
    cursor: pointer;
    font-size: 14px;
}

.reset {
    background: #6c757d;
}

.submit {
    background: #28a745;
}

button:hover {
    opacity: 0.9;
}
