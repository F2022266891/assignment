<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Assinment #2 web technlogy</title>
<style>
body{
    background-color: rgb(147, 179, 193);
}
header{
    background-color: rgb(97, 92, 102);
    color: antiquewhite;
    text-align: center;

}
button{
    button-center: center;
}
</style>
</head>
<body>
    <header>
        <h1>Sajjad Ali</h1>
        <h2>Web Developer</h2>
        <p>"Create the bst and strong web sites ."</p>
    </header>

    <section id="education">
        <h2>Education</h2>
        <ul>
            <li>BS in Computer Science,  UMT,2026</li>
            <li>Intermediate, General M.Musa collage, 2021</li>
            <li>Matriculation, Hzara society high School, 2019</li>
        </ul>
    </section>

    <section id="skills">
        <h2>Skills</h2>
        <ul>
            
            <li>HTML & CSS</li>
            <li>JavaScript</li>
            <li>c++ </li>
            <li>pyton</li>
        </ul>
    </section>

    <section id="experience">
        <h2>Experience</h2>
        <ul>
            <li>work with different compines 2021-2024</li>
            <li>Create many websites for local hotels and shopes </li>
        </ul>
    </section>

    <section id="projects">
        <h2>Complete Projects</h2>
        <ul>
            <li>
                <h3>Project </h3>
                <p>Description of project .</p>
                <a href="abc" target="_blank">View Project</a>
            </li>
            
        </ul>
    </section>

    <section id="contact">
        <h2>Contact Me</h2>
        <form id="contactForm">
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" required><br><br>
            <label for="contectnumber">Contect Number:</label>
            <input type="text" id="contectnumber" name="contectnumber" required><br><br>
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required><br><br>
            <label for="message">Message:</label>
            <textarea id="message" name="message" required></textarea><br><br>
            <button type="submit">Send</button>
        </form>
    </section>
    <script>
        document.addEventListener("DOMContentLoaded", function() {
            document.getElementById("contactForm").addEventListener("submit", function(event) {
                event.preventDefault(); // Prevent the form from submitting

                // Get form values
                const name = document.getElementById("name").value;
                const contactNumber = document.getElementById("contactnumber").value;
                const email = document.getElementById("email").value;
                const message = document.getElementById("message").value;

                // Basic form validation
                if (!name || !contactNumber || !email || !message) {
                    alert("Please fill in all fields.");
                    return;
                }

                // Email validation
                const emailPattern = /^[a-zA-Z0-9._-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,6}$/;
                if (!emailPattern.test(email)) {
                    alert("Please enter a valid email address.");
                    return;
                }

                alert("Form submitted successfully!\n" +
                      "Name: " + name + "\n" +
                      "Contact Number: " + contactNumber + "\n" +
                      "Email: " + email + "\n" +
                      "Message: " + message);
            });
        });
    </script>

</body>
</html>

