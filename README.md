<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Feedback form</title>
    <style>

        *
        {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body
        {
            font-family: Arial, Helvetica, sans-serif;
            background: #f5f5f5;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100svh;
            
        }
        .feedback_form
        {
            background-color: rgb(97,97,97);
            width: 400px;  
            padding: 20px;
            border-radius: 7px; 
        }
        h2
        {
            text-align: center;
            margin-bottom: 20px;
        }
        input , select,textarea
        {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border: 2px solid #ccc;
            border-radius: 8px;
            font-size: 14px;
        }
        textarea
        {
            min-height: 100px;
        }
        button
        {
            margin-top: 20px;
            width: 100%;
            padding: 10px;
            background-color: #28a745;
            border: none;
            color: white;
            font-size: 16px;
            border-radius: 6px;
            cursor: pointer;
        }
        button:hover
        {
            background-color: #218838;
        }
        
    </style>
</head>
<body>
    <div class="feedback_form">
        <h2>Shopping site feedback</h2>
        <form>
            <label for="Name">Name:</label>
            <input type="text" id="name" name="Name" placeholder="Your Name" required/>

            <label for="email">Email</label>
            <input type="email" id="email" placeholder="your email" required/>

            <label for="rating">Over all rating</label>
            <select id="rating" name="rating" required>
                <option value="">--Select--</option>
                <option value="5">Excellent</option>
                <option value="4">Good</option>
                <option value="3">Average</option>
                <option value="2">Poor</option>
                <option value="1">Very Poor</option>
            </select>

            <label for="Comments">Comments</label>
            <textarea id="comments" name="comments" placeholder="Write your feedback here...."></textarea>


            <button onclick="Feedback()">Submit feedback</button>

            <a href="Shop_ease.html">Home</a>
            
        </form>
    </div>

    <script>

        function Feedback()
        {
            alert("Feedback submited sucessfully");
        }

    </script>
</body>
</html>
