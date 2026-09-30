# smartnet-solution
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>SmartNet Solutions - ICT Project</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            scroll-behavior: smooth;
        }

        body {
            font-family: Arial, sans-serif;
            background: #f4f6f8;
            color: #222;
            line-height: 1.6;
        }

        /* ================= NAVIGATION ================= */

        nav {
            background: #0b1f33;
            padding: 15px 30px;
            position: sticky;
            top: 0;
            z-index: 1000;
            display: flex;
            justify-content: space-between;
            align-items: center;
            box-shadow: 0 2px 8px rgba(0,0,0,0.3);
        }

        .logo {
            color: white;
            font-size: 23px;
            font-weight: bold;
        }

        .menu {
            display: flex;
            list-style: none;
            gap: 20px;
        }

        .menu a {
            color: white;
            text-decoration: none;
            font-weight: bold;
        }

        .menu a:hover {
            color: #00bfff;
        }

        /* ================= GENERAL ================= */

        section {
            padding: 80px 30px;
            min-height: 70vh;
        }

        .container {
            max-width: 1100px;
            margin: auto;
        }

        h1 {
            font-size: 48px;
            margin-bottom: 20px;
        }

        h2 {
            text-align: center;
            font-size: 35px;
            margin-bottom: 30px;
            color: #0b1f33;
        }

        h3 {
            margin-bottom: 15px;
        }

        p {
            margin-bottom: 15px;
        }

        /* ================= HOME ================= */

        #home {
            background: linear-gradient(to right, #007bff, #00bfff);
            color: white;
            text-align: center;
            min-height: 90vh;
            display: flex;
            align-items: center;
        }

        .home-content {
            width: 100%;
        }

        .home-content p {
            max-width: 800px;
            margin: auto;
            font-size: 19px;
        }

        .btn {
            display: inline-block;
            background: #0b1f33;
            color: white;
            text-decoration: none;
            padding: 13px 25px;
            border-radius: 6px;
            margin-top: 20px;
            font-weight: bold;
        }

        .btn:hover {
            background: #00bfff;
        }

        /* ================= PROJECT TITLE ================= */

        #project-title {
            background: white;
            text-align: center;
        }

        .title-box {
            background: #eef7ff;
            padding: 40px;
            border-radius: 12px;
            max-width: 900px;
            margin: auto;
            box-shadow: 0 4px 12px rgba(0,0,0,0.1);
        }

        .title-box h3 {
            color: #007bff;
            font-size: 28px;
        }

        /* ================= ABOUT ================= */

        #about {
            background: #f4f6f8;
        }

        .about-text {
            max-width: 900px;
            margin: auto;
            font-size: 18px;
        }

        /* ================= OBJECTIVES ================= */

        #objectives {
            background: white;
        }

        .objectives {
            max-width: 800px;
            margin: auto;
        }

        .objectives li {
            margin: 12px 0;
            font-size: 18px;
        }

        /* ================= SERVICES ================= */

        #services {
            background: #eaf5ff;
        }

        .cards {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 25px;
        }

        .card {
            background: white;
            width: 280px;
            padding: 30px;
            border-radius: 10px;
            text-align: center;
            box-shadow: 0 4px 12px rgba(0,0,0,0.15);
        }

        .card:hover {
            transform: translateY(-5px);
            transition: 0.3s;
        }

        .card h3 {
            color: #007bff;
        }

        /* ================= FEATURES ================= */

        #features {
            background: white;
        }

        .features-list {
            max-width: 900px;
            margin: auto;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }

        .feature {
            padding: 25px;
            background: #f4f6f8;
            border-left: 5px solid #007bff;
            border-radius: 5px;
        }

        /* ================= HOW IT WORKS ================= */

        #how {
            background: #eef7ff;
        }

        .steps {
            max-width: 800px;
            margin: auto;
        }

        .step {
            background: white;
            padding: 20px;
            margin: 15px 0;
            border-radius: 8px;
            box-shadow: 0 2px 7px rgba(0,0,0,0.1);
        }

        .step span {
            background: #007bff;
            color: white;
            padding: 8px 12px;
            border-radius: 50%;
            margin-right: 10px;
        }

        /* ================= PROJECT DETAILS ================= */

        #project {
            background: white;
        }

        .project-info {
            max-width: 900px;
            margin: auto;
        }

        .project-info table {
            width: 100%;
            border-collapse: collapse;
        }

        .project-info th,
        .project-info td {
            border: 1px solid #ccc;
            padding: 15px;
            text-align: left;
        }

        .project-info th {
            background: #0b1f33;
            color: white;
        }

        /* ================= TEAM ================= */

        #team {
            background: #f4f6f8;
            text-align: center;
        }

        /* ================= FAQ ================= */

        #faq {
            background: white;
        }

        .faq-box {
            max-width: 800px;
            margin: auto;
        }

        details {
            background: #f4f6f8;
            margin: 10px 0;
            padding: 15px;
            border-radius: 5px;
        }

        summary {
            font-weight: bold;
            cursor: pointer;
        }

        /* ================= CONTACT ================= */

        #contact {
            background: #0b1f33;
            color: white;
            text-align: center;
        }

        #contact h2 {
            color: white;
        }

        /* ================= FOOTER ================= */

        footer {
            background: #06121f;
            color: white;
            text-align: center;
            padding: 20px;
        }

        /* ================= MOBILE ================= */

        @media (max-width: 900px) {

            nav {
                flex-direction: column;
                gap: 15px;
            }

            .menu {
                flex-wrap: wrap;
                justify-content: center;
                gap: 10px;
            }

            h1 {
                font-size: 36px;
            }
        }
    </style>
</head>

<body>

<!-- ================= NAVIGATION ================= -->

<nav>

    <div class="logo">
        SmartNet Solutions
    </div>

    <ul class="menu">
        <li><a href="#home">Home</a></li>
        <li><a href="#project-title">Project Title</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#objectives">Objectives</a></li>
        <li><a href="#services">Services</a></li>
        <li><a href="#features">Features</a></li>
        <li><a href="#how">How It Works</a></li>
        <li><a href="#project">Project Details</a></li>
        <li><a href="#team">Team</a></li>
        <li><a href="#faq">FAQ</a></li>
        <li><a href="#contact">Contact</a></li>
    </ul>

</nav>


<!-- ================= HOME ================= -->

<section id="home">

    <div class="home-content">

        <h1>SMARTNET SOLUTIONS</h1>

        <p>
            Provision of Affordable and Reliable Wi-Fi Networking
            Services to Residential Estates and Student Hostels.
        </p>

        <a href="#services" class="btn">
            Explore Our Services
        </a>

    </div>

</section>


<!-- ================= PROJECT TITLE ================= -->

<section id="project-title">

    <div class="container">

        <h2>Project Title</h2>

        <div class="title-box">

            <h3>
                Provision of Affordable and Reliable Wi-Fi
                Networking Services to Residential Estates
                and Student Hostels
            </h3>

            <p>
                SmartNet Solutions is an ICT networking project
                designed to provide affordable, reliable and
                secure internet connectivity to students,
                households and residential communities.
            </p>

        </div>

    </div>

</section>


<!-- ================= ABOUT ================= -->

<section id="about">

    <div class="container">

        <h2>About the Project</h2>

        <div class="about-text">

            <p>
                SmartNet Solutions focuses on designing,
                installing and maintaining reliable Wi-Fi
                networks for residential estates and student
                hostels.
            </p>

            <p>
                The project aims to address challenges such as
                expensive internet packages, poor network
                coverage, unreliable connectivity and lack
                of professional network management.
            </p>

            <p>
                The solution combines networking equipment,
                internet connectivity, hotspot management
                and technical support to provide users with
                dependable internet access.
            </p>

        </div>

    </div>

</section>


<!-- ================= OBJECTIVES ================= -->

<section id="objectives">

    <div class="container">

        <h2>Project Objectives</h2>

        <div class="objectives">

            <ul>

                <li>
                    To provide affordable internet connectivity.
                </li>

                <li>
                    To improve Wi-Fi coverage in residential areas.
                </li>

                <li>
                    To provide reliable internet services to students.
                </li>

                <li>
                    To install secure and professionally managed networks.
                </li>

                <li>
                    To provide technical support and network maintenance.
                </li>

                <li>
                    To create employment opportunities for ICT technicians.
                </li>

            </ul>

        </div>

    </div>

</section>


<!-- ================= SERVICES ================= -->

<section id="services">

    <div class="container">

        <h2>Services Offered</h2>

        <div class="cards">

            <div class="card">

                <h3>Wi-Fi Installation</h3>

                <p>
                    Professional installation and configuration
                    of Wi-Fi networks in hostels and residential
                    estates.
                </p>

            </div>


            <div class="card">

                <h3>Network Design</h3>

                <p>
                    Designing network infrastructure according
                    to customer requirements and building layout.
                </p>

            </div>


            <div class="card">

                <h3>Hotspot Management</h3>

                <p>
                    Management of user access, authentication,
                    bandwidth and internet usage.
                </p>

            </div>


            <div class="card">

                <h3>Network Maintenance</h3>

                <p>
                    Troubleshooting, repair and maintenance
                    of network equipment.
                </p>

            </div>


            <div class="card">

                <h3>Customer Support</h3>

                <p>
                    Technical assistance and customer support
                    for internet connectivity problems.
                </p>

            </div>


            <div class="card">

                <h3>Network Security</h3>

                <p>
                    Configuration of secure Wi-Fi access,
                    passwords and network protection.
                </p>

            </div>

        </div>

    </div>

</section>


<!-- ================= FEATURES ================= -->

<section id="features">

    <div class="container">

        <h2>Project Features</h2>

        <div class="features-list">

            <div class="feature">
                <h3>Reliable Connectivity</h3>
                <p>
                    Provides stable internet access to users.
                </p>
            </div>

            <div class="feature">
                <h3>Affordable Packages</h3>
                <p>
                    Offers internet packages designed for
                    students and residential users.
                </p>
            </div>

            <div class="feature">
                <h3>User Authentication</h3>
                <p>
                    Controls who can access the network.
                </p>
            </div>

            <div class="feature">
                <h3>Bandwidth Management</h3>
                <p>
                    Helps manage internet usage and network
                    performance.
                </p>
            </div>

            <div class="feature">
                <h3>Network Monitoring</h3>
                <p>
                    Allows administrators to monitor network
                    performance.
                </p>
            </div>

            <div class="feature">
                <h3>Technical Support</h3>
                <p>
                    Provides assistance whenever network
                    problems occur.
                </p>
            </div>

        </div>

    </div>

</section>


<!-- ================= HOW IT WORKS ================= -->

<section id="how">

    <div class="container">

        <h2>How the Service Works</h2>

        <div class="steps">

            <div class="step">
                <span>1</span>
                Customer contacts SmartNet Solutions.
            </div>

            <div class="step">
                <span>2</span>
                Our technician assesses the location.
            </div>

            <div class="step">
                <span>3</span>
                We design the appropriate network.
            </div>

            <div class="step">
                <span>4</span>
                Networking equipment is installed.
            </div>

            <div class="step">
                <span>5</span>
                The network is configured and tested.
            </div>

            <div class="step">
                <span>6</span>
                Customers receive internet access.
            </div>

            <div class="step">
                <span>7</span>
                Continuous technical support is provided.
            </div>

        </div>

    </div>

</section>


<!-- ================= PROJECT DETAILS ================= -->

<section id="project">

    <div class="container">

        <h2>Project Details</h2>

        <div class="project-info">

            <table>

                <tr>
                    <th>Project</th>
                    <td>SmartNet Solutions</td>
                </tr>

                <tr>
                    <th>Project Type</th>
                    <td>ICT Networking Project</td>
                </tr>

                <tr>
                    <th>Main Service</th>
                    <td>Wi-Fi Networking</td>
                </tr>

                <tr>
                    <th>Target Customers</th>
                    <td>
                        Students, Hostels, Residential Estates
                        and Households
                    </td>
                </tr>

                <tr>
                    <th>Location</th>
                    <td>Kakamega, Kenya</td>
                </tr>

                <tr>
                    <th>Course</th>
                    <td>Diploma in Computer Science</td>
                </tr>

                <tr>
                    <th>Institution</th>
                    <td>Sigalagala National Polytechnic</td>
                </tr>

                <tr>
                    <th>Technology</th>
                    <td>
                        Wi-Fi, Routers, Access Points,
                        Networking and Hotspot Management
                    </td>
                </tr>

            </table>

        </div>

    </div>

</section>


<!-- ================= TEAM ================= -->

<section id="team">

    <div class="container">

        <h2>Project Team</h2>

        <p>
            <strong>Project Developer:</strong>
            Brian Koech
        </p>

        <p>
            <strong>Course:</strong>
            Diploma in Computer Science
        </p>

        <p>
            <strong>Institution:</strong>
            Sigalagala National Polytechnic
        </p>

    </div>

</section>


<!-- ================= FAQ ================= -->

<section id="faq">

    <div class="container">

        <h2>Frequently Asked Questions</h2>

        <div class="faq-box">

            <details>

                <summary>
                    Who can use SmartNet Solutions?
                </summary>

                <p>
                    Students, hostels, households and
                    residential estates can use the service.
                </p>

            </details>


            <details>

                <summary>
                    Do you install Wi-Fi?
                </summary>

                <p>
                    Yes. We provide Wi-Fi installation,
                    configuration and maintenance.
                </p>

            </details>


            <details>

                <summary>
                    Do you provide technical support?
                </summary>

                <p>
                    Yes. Customers receive technical support
                    for network-related problems.
                </p>

            </details>


            <details>

                <summary>
                    Is the network secure?
                </summary>

                <p>
                    Network security measures such as secure
                    authentication and access control can be
                    implemented.
                </p>

            </details>

        </div>

    </div>

</section>


<!-- ================= CONTACT ================= -->

<section id="contact">

    <div class="container">

        <h2>Contact Us</h2>

        <p>
            Get in touch with SmartNet Solutions for
            networking services and technical support.
        </p>

        <p>
            Email: smartnetsolutions@example.com
        </p>

        <p>
            Phone: +254 700 000 000
        </p>

        <p>
            Location: Kakamega, Kenya
        </p>

        <a href="#home" class="btn">
            Back to Home
        </a>

    </div>

</section>


<!-- ================= FOOTER ================= -->

<footer>

    <p>
        © 2026 SmartNet Solutions.
        All Rights Reserved.
    </p>