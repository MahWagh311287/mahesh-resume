<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mahesh Waghmare - Cloud & DevOps Engineer</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&family=Montserrat:wght@400;600;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary: #3498db;
            --secondary: #2ecc71;
            --dark: #2c3e50;
            --light: #ecf0f1;
            --accent: #e74c3c;
            --shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            --transition: all 0.3s ease;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Poppins', sans-serif;
            line-height: 1.6;
            color: #333;
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            padding: 0;
            margin: 0;
        }
        
        .container {
            max-width: 1100px;
            margin: 0 auto;
            padding: 20px;
            background-color: white;
            box-shadow: var(--shadow);
            border-radius: 10px;
            margin-top: 30px;
            margin-bottom: 30px;
            position: relative;
            overflow: hidden;
        }
        
        .container::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 10px;
            background: linear-gradient(90deg, var(--primary), var(--secondary), var(--accent));
        }
        
        header {
            display: flex;
            align-items: center;
            padding: 30px 0;
            border-bottom: 1px solid rgba(0, 0, 0, 0.1);
            margin-bottom: 30px;
            animation: fadeIn 1s ease;
        }
        
        .profile-img {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            object-fit: cover;
            border: 5px solid white;
            box-shadow: var(--shadow);
            margin-right: 30px;
            transition: var(--transition);
        }
        
        .profile-img:hover {
            transform: scale(1.05);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
        }
        
        .header-content {
            flex: 1;
        }
        
        h1 {
            font-family: 'Montserrat', sans-serif;
            font-size: 2.5rem;
            color: var(--dark);
            margin-bottom: 5px;
            background: linear-gradient(90deg, var(--primary), var(--secondary));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            display: inline-block;
        }
        
        .title {
            font-size: 1.2rem;
            color: var(--primary);
            margin-bottom: 15px;
            font-weight: 600;
        }
        
        .contact-info {
            display: flex;
            flex-wrap: wrap;
            gap: 15px;
            margin-top: 10px;
        }
        
        .contact-item {
            display: flex;
            align-items: center;
            color: #555;
            font-size: 0.9rem;
        }
        
        .contact-item i {
            margin-right: 8px;
            color: var(--primary);
        }
        
        section {
            margin-bottom: 40px;
            animation: fadeInUp 0.8s ease;
        }
        
        h2 {
            font-family: 'Montserrat', sans-serif;
            font-size: 1.8rem;
            color: var(--dark);
            margin-bottom: 20px;
            padding-bottom: 10px;
            border-bottom: 2px solid var(--light);
            position: relative;
        }
        
        h2::after {
            content: '';
            position: absolute;
            bottom: -2px;
            left: 0;
            width: 100px;
            height: 2px;
            background: linear-gradient(90deg, var(--primary), var(--secondary));
        }
        
        h3 {
            font-size: 1.3rem;
            color: var(--dark);
            margin-bottom: 5px;
        }
        
        .experience-header {
            display: flex;
            justify-content: space-between;
            margin-bottom: 10px;
        }
        
        .company {
            font-weight: 600;
            color: var(--primary);
        }
        
        .date {
            color: #777;
            font-size: 0.9rem;
        }
        
        p {
            margin-bottom: 15px;
            color: #555;
        }
        
        ul {
            margin-bottom: 20px;
            padding-left: 20px;
        }
        
        li {
            margin-bottom: 8px;
            position: relative;
            list-style-type: none;
        }
        
        li::before {
            content: '▹';
            position: absolute;
            left: -20px;
            color: var(--secondary);
        }
        
        .skills-container {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin-top: 15px;
        }
        
        .skill {
            background-color: var(--light);
            padding: 8px 15px;
            border-radius: 20px;
            font-size: 0.9rem;
            color: var(--dark);
            transition: var(--transition);
        }
        
        .skill:hover {
            background: linear-gradient(90deg, var(--primary), var(--secondary));
            color: white;
            transform: translateY(-3px);
        }
        
        .project-item {
            margin-bottom: 25px;
            padding: 20px;
            border-radius: 8px;
            background-color: white;
            box-shadow: var(--shadow);
            transition: var(--transition);
            border-left: 4px solid var(--primary);
        }
        
        .project-item:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
            border-left: 4px solid var(--secondary);
        }
        
        .project-title {
            font-weight: 600;
            color: var(--dark);
            margin-bottom: 10px;
            display: flex;
            align-items: center;
        }
        
        .project-title i {
            margin-right: 10px;
            color: var(--primary);
        }
        
        .certificate-item {
            display: flex;
            align-items: center;
            margin-bottom: 15px;
            padding: 15px;
            background-color: var(--light);
            border-radius: 8px;
            transition: var(--transition);
        }
        
        .certificate-item:hover {
            background-color: #e0e0e0;
            transform: translateX(5px);
        }
        
        .certificate-item i {
            font-size: 1.5rem;
            color: var(--accent);
            margin-right: 15px;
        }
        
        .progress-container {
            width: 100%;
            background-color: #e0e0e0;
            border-radius: 5px;
            margin: 20px 0;
            overflow: hidden;
        }
        
        .progress-bar {
            height: 10px;
            background: linear-gradient(90deg, var(--primary), var(--secondary));
            border-radius: 5px;
            width: 0;
            transition: width 1s ease;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        @media (max-width: 768px) {
            header {
                flex-direction: column;
                text-align: center;
            }
            
            .profile-img {
                margin-right: 0;
                margin-bottom: 20px;
            }
            
            .contact-info {
                justify-content: center;
            }
            
            .experience-header {
                flex-direction: column;
            }
            
            .date {
                margin-top: 5px;
            }
        }
        
        /* Toggle switch for dark mode */
        .theme-switch {
            position: fixed;
            top: 20px;
            right: 20px;
            z-index: 100;
        }
        
        .switch {
            position: relative;
            display: inline-block;
            width: 60px;
            height: 34px;
        }
        
        .switch input {
            opacity: 0;
            width: 0;
            height: 0;
        }
        
        .slider {
            position: absolute;
            cursor: pointer;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background-color: #ccc;
            transition: .4s;
            border-radius: 34px;
        }
        
        .slider:before {
            position: absolute;
            content: "";
            height: 26px;
            width: 26px;
            left: 4px;
            bottom: 4px;
            background-color: white;
            transition: .4s;
            border-radius: 50%;
        }
        
        input:checked + .slider {
            background: linear-gradient(90deg, var(--primary), var(--secondary));
        }
        
        input:checked + .slider:before {
            transform: translateX(26px);
        }
        
        .fa-moon, .fa-sun {
            position: absolute;
            top: 50%;
            transform: translateY(-50%);
            color: white;
            font-size: 12px;
        }
        
        .fa-moon {
            left: 10px;
        }
        
        .fa-sun {
            right: 10px;
        }
        
        /* Dark mode styles */
        body.dark-mode {
            background: linear-gradient(135deg, #1a1a2e 0%, #16213e 100%);
            color: #f0f0f0;
        }
        
        .dark-mode .container {
            background-color: #1e293b;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
        }
        
        .dark-mode h1, .dark-mode h2, .dark-mode h3, .dark-mode .company {
            color: #f8fafc;
        }
        
        .dark-mode p, .dark-mode .contact-item, .dark-mode .date {
            color: #cbd5e1;
        }
        
        .dark-mode .project-item, .dark-mode .certificate-item {
            background-color: #334155;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }
        
        .dark-mode .skill {
            background-color: #475569;
            color: #f8fafc;
        }
        
        .dark-mode li::before {
            color: var(--primary);
        }
    </style>
</head>
<body>
    <div class="theme-switch">
        <label class="switch">
            <input type="checkbox" id="theme-toggle">
            <span class="slider">
                <i class="fas fa-moon"></i>
                <i class="fas fa-sun"></i>
            </span>
        </label>
    </div>

    <div class="container">
        <header>
            <img src="https://via.placeholder.com/150" alt="Mahesh Waghmare" class="profile-img" id="profile-pic">
            <div class="header-content">
                <h1>Mahesh Waghmare</h1>
                <div class="title">Cloud & DevOps Engineer</div>
                <div class="contact-info">
                    <div class="contact-item">
                        <i class="fas fa-phone"></i> 7261938383
                    </div>
                    <div class="contact-item">
                        <i class="fas fa-envelope"></i> mahesh.v.waghmare311287@gmail.com
                    </div>
                    <div class="contact-item">
                        <i class="fas fa-map-marker-alt"></i> Pune, Maharashtra
                    </div>
                    <div class="contact-item">
                        <i class="fab fa-linkedin"></i> linkedin.com/in/mahesh-waghmare
                    </div>
                    <div class="contact-item">
                        <i class="fab fa-github"></i> github.com/maheshwaghmare
                    </div>
                </div>
            </div>
        </header>

        <section id="summary">
            <h2><i class="fas fa-user-tie"></i> Professional Summary</h2>
            <div class="progress-container">
                <div class="progress-bar" id="summary-progress"></div>
            </div>
            <p>
                <i class="fas fa-cloud" style="color: var(--primary); margin-right: 8px;"></i>
                Proficient in Administrating Azure IaaS/PaaS services like compute Azure Virtual Machines, Web and Worker roles,
                VNET, Network services, Azure DevOps, SQL Databases, Storages, Azure Active Directory, Monitoring, Autoscaling,
                PowerShell Automation, Azure Search, DNS, VPN.
            </p>
            <p>
                <i class="fas fa-server" style="color: var(--primary); margin-right: 8px;"></i>
                Extensive experience in migrating on-premises applications to Azure and configured VNETs and subnets as per the
                project requirement.
            </p>
            <p>
                <i class="fas fa-code" style="color: var(--primary); margin-right: 8px;"></i>
                Hands on experience in writing Terraform Tool to deploy, update and delete multiple resources in Azure.
            </p>
            <p>
                <i class="fas fa-network-wired" style="color: var(--primary); margin-right: 8px;"></i>
                Experience in Azure IaaS - Virtual machines, VM Scale Sets, Load Balancer, Traffic Manager, Virtual Networks, SQL,
                Resource Groups and Cloud Services.
            </p>
            <p>
                <i class="fas fa-shield-alt" style="color: var(--primary); margin-right: 8px;"></i>
                Extensive involvement in Azure Backup, Azure Policies, Azure Key Vault, Salt Stack and Tagging.
            </p>
            <p>
                <i class="fas fa-cogs" style="color: var(--primary); margin-right: 8px;"></i>
                Experience in Azure Platform Development, Deployment Concepts., hosted Cloud Services, platform services and
                close interface with Windows Azure Multi-Factor Authentications.
            </p>
            <p>
                <i class="fas fa-sync-alt" style="color: var(--primary); margin-right: 8px;"></i>
                Experience in CI/CD tools like Azure Devops.
            </p>
        </section>

        <section id="certificates">
            <h2><i class="fas fa-certificate"></i> Certifications</h2>
            <div class="progress-container">
                <div class="progress-bar" id="certs-progress"></div>
            </div>
            <div class="certificate-item">
                <i class="fab fa-aws"></i>
                <div>
                    <strong>AWS Certified Solutions Architect - Associate</strong>
                    <p>Issued: 2023 | Credential ID: AWS-ASA-12345</p>
                </div>
            </div>
            <div class="certificate-item">
                <i class="fab fa-microsoft"></i>
                <div>
                    <strong>Microsoft Certified: Azure Administrator Associate</strong>
                    <p>Issued: 2022 | Credential ID: MS-AZ104-67890</p>
                </div>
            </div>
        </section>

        <section id="skills">
            <h2><i class="fas fa-laptop-code"></i> Technical Skills</h2>
            <div class="progress-container">
                <div class="progress-bar" id="skills-progress"></div>
            </div>
            <div class="skills-container">
                <div class="skill"><i class="fab fa-linux"></i> Linux</div>
                <div class="skill"><i class="fab fa-microsoft"></i> Azure</div>
                <div class="skill"><i class="fab fa-aws"></i> AWS</div>
                <div class="skill"><i class="fas fa-code"></i> Terraform</div>
                <div class="skill"><i class="fas fa-robot"></i> Ansible</div>
                <div class="skill"><i class="fas fa-project-diagram"></i> Azure Pipeline</div>
                <div class="skill"><i class="fab fa-docker"></i> Docker</div>
                <div class="skill"><i class="fab fa-git-alt"></i> Git</div>
                <div class="skill"><i class="fas fa-database"></i> Azure Repo</div>
                <div class="skill"><i class="fas fa-chart-line"></i> Prometheus</div>
                <div class="skill"><i class="fas fa-chart-pie"></i> Grafana</div>
                <div class="skill"><i class="fas fa-desktop"></i> Zabbix</div>
                <div class="skill"><i class="fas fa-terminal"></i> Bash Scripting</div>
                <div class="skill"><i class="fas fa-database"></i> HANA Database</div>
                <div class="skill"><i class="fas fa-database"></i> MySQL</div>
                <div class="skill"><i class="fas fa-server"></i> Apache Tomcat</div>
                <div class="skill"><i class="fas fa-server"></i> Nginx</div>
                <div class="skill"><i class="fas fa-cloud"></i> VMWARE</div>
                <div class="skill"><i class="fas fa-cloud"></i> KVM</div>
            </div>
        </section>

        <section id="experience">
            <h2><i class="fas fa-briefcase"></i> Professional Experience</h2>
            <div class="progress-container">
                <div class="progress-bar" id="exp-progress"></div>
            </div>
            
            <div class="experience-item">
                <div class="experience-header">
                    <h3 class="company">Acuiti Labs</h3>
                    <span class="date">07/2022 - Present</span>
                </div>
                <p><strong>Senior Associate | Pune, Maharashtra</strong></p>
                <ul>
                    <li>Designed and implemented Azure Solutions across a range of cloud models like SaaS, PaaS, IaaS, and integrated on-premises, on-demand workloads with the Azure public cloud.</li>
                    <li>Worked on Microservices for Continuous Delivery environment using Azure, Docker. Involved in setting up a Microservice architecture for application development and Implemented high availability with Azure Classic and Azure Resource Manager deployment models.</li>
                    <li>Extensively worked on Building and Installing servers, creating multiple resources like in Azure through Azure Portal and provisioned them using Terraform templates. Also worked on Virtual networks, Azure Custom security, endpoint security and firewall.</li>
                    <li>Worked in setting up Azure Virtual Appliances (VMs) to meet security requirements as software-based appliance functions(firewall).</li>
                    <li>Constructed and Installed servers through Azure Portal. Migrating On-premises virtual machines to Azure Resource Manager(ARM) Subscription with Azure Site Recovery.</li>
                    <li>Developed and designed Azure DevOps pipeline to manage the resources across multiple subscription in Azure.</li>
                    <li>Worked with Version Control, Build & Release Management and Deployments of the Solutions to the DEV, QA & PROD Environments leveraging Azure DevOps/VSTS principles/process (CI/CD) and toolsets of Visual Studio, Application Insights, Log Analytics.</li>
                    <li>Provisioning servers/instances using infrastructure as code such as Terraform and CloudFormation. Code is stored in a private repository and constantly updated.</li>
                    <li>Worked on Terraform templates also for provisioning virtual networks, subnets, VM Scale sets, Load balancers, and NAT rules and used terraform graph to visualize execution plan using the graph command.</li>
                    <li>Connections between on-premises data centers and Azure cloud by tunneling.</li>
                    <li>Integrated Ansible with Jenkins to provide automation, continuous integration & Continuous Deployment through Jenkins and wrote Playbooks to automate Ansible servers using YAML scripting. Implemented Jenkins Workflow and Plugins for repeatable deployments of multi-tier applications, artifacts, and services to Docker.</li>
                    <li>Developed GIT hooks for the local repository, code commit and remote repository, code push functionality and on GitHub.</li>
                    <li>Used Grafana for log aggregation and analysis on different application servers.</li>
                    <li>Experience in JIRA for ticketing and as well as defect tracking system and configure various workflows, customizations and plug-ins for JIRA bug/issue tracker.</li>
                    <li>HANA Database installation and monitoring by HANA Studio.</li>
                </ul>
            </div>
            
            <div class="experience-item">
                <div class="experience-header">
                    <h3 class="company">Meganet India Pvt Ltd</h3>
                    <span class="date">01/2022 - 07/2022</span>
                </div>
                <p><strong>Senior Linux Administrator | Mumbai, Maharashtra</strong></p>
                <ul>
                    <li>Responsible for installation, configuration and administration of Red Hat Enterprise Linux, Ubuntu, CentoOS on x86 architecture.</li>
                    <li>Setting up, configuring and troubleshooting NFS, DNS, DHCP, SFTP, NTP and Samba servers on different multi-platforms (Windows, Linux).</li>
                    <li>Administered RedHat Enterprise Linux 7.x/8.x/9x and Ubuntu 20.04LTS/22.04LTS servers by testing, tuning, upgrading, patching and troubleshooting both Physical & Virtual server problems.</li>
                    <li>Installed and configured Disk and file system management using Logical Volume Manager (LVM) for Linux systems.</li>
                    <li>Local and remote administering of servers, routers and networks using Telnet and SSH login using SSH keygen tools for password-less setup and agent forwarding on Linux.</li>
                    <li>Responsible for setting up Cronjobs scripts on production server.</li>
                    <li>Configured LDAP on RedHat for authorization and authentication by configuring LDAP server which is used for authentication using its database.</li>
                    <li>Managing services, maintaining and managing log files, monitoring events, logs and troubleshooting system problems using Zabbix tool and resolve for any reported issues.</li>
                </ul>
            </div>
            
            <div class="experience-item">
                <div class="experience-header">
                    <h3 class="company">Mphasis</h3>
                    <span class="date">01/2021 - 08/2021</span>
                </div>
                <p><strong>Linux Administrator | Pune, Maharashtra</strong></p>
            </div>
            
            <div class="experience-item">
                <div class="experience-header">
                    <h3 class="company">Wipro Technology</h3>
                    <span class="date">11/2018 - 01/2021</span>
                </div>
                <p><strong>Linux Administrator | Pune, Maharashtra</strong></p>
            </div>
            
            <div class="experience-item">
                <div class="experience-header">
                    <h3 class="company">Tata Communications Payment Solution Ltd</h3>
                    <span class="date">03/2015 - 10/2017</span>
                </div>
                <p><strong>Linux Systems Administrator | Pune, Maharashtra</strong></p>
            </div>
        </section>

        <section id="education">
            <h2><i class="fas fa-graduation-cap"></i> Education</h2>
            <div class="progress-container">
                <div class="progress-bar" id="edu-progress"></div>
            </div>
            <div class="education-item">
                <h3>Marathwada Mitra Mandal Polytechnic</h3>
                <p>Electronics and Telecommunications | 07/2012</p>
                <p>Pune, Maharashtra</p>
            </div>
        </section>

        <section id="projects">
            <h2><i class="fas fa-project-diagram"></i> Projects</h2>
            <div class="progress-container">
                <div class="progress-bar" id="projects-progress"></div>
            </div>
            <div class="project-item">
                <div class="project-title">
                    <i class="fas fa-shopping-cart"></i>
                    <span>E-commerce Website Migration to Azure</span>
                </div>
                <p>Migrated a high-traffic e-commerce platform from on-premises infrastructure to Azure cloud, improving scalability and reducing downtime by 60%. Implemented Azure Kubernetes Service (AKS) for container orchestration and Azure Front Door for global load balancing.</p>
                <p><strong>Technologies:</strong> Azure, Kubernetes, Terraform, CI/CD Pipelines</p>
            </div>
            <div class="project-item">
                <div class="project-title">
                    <i class="fas fa-database"></i>
                    <span>Automated Infrastructure Deployment</span>
                </div>
                <p>Developed Terraform modules to automate the deployment of complex infrastructure across multiple Azure subscriptions. Reduced deployment time from days to minutes and improved consistency across environments.</p>
                <p><strong>Technologies:</strong> Terraform, Azure Resource Manager, PowerShell</p>
            </div>
            <div class="project-item">
                <div class="project-title">
                    <i class="fas fa-shield-alt"></i>
                    <span>Security Hardening for Linux Servers</span>
                </div>
                <p>Created Ansible playbooks to automate security hardening of Linux servers across the enterprise, achieving compliance with CIS benchmarks. Implemented automated vulnerability scanning and patch management.</p>
                <p><strong>Technologies:</strong> Ansible, CIS Benchmarks, Bash Scripting</p>
            </div>
        </section>
    </div>

    <script>
        // Dark mode toggle
        const themeToggle = document.getElementById('theme-toggle');
        const body = document.body;
        
        // Check for saved user preference or use system preference
        if (localStorage.getItem('darkMode') === 'enabled' || 
            (!localStorage.getItem('darkMode') && window.matchMedia('(prefers-color-scheme: dark)').matches)) {
            body.classList.add('dark-mode');
            themeToggle.checked = true;
        }
        
        themeToggle.addEventListener('change', function() {
            if (this.checked) {
                body.classList.add('dark-mode');
                localStorage.setItem('darkMode', 'enabled');
            } else {
                body.classList.remove('dark-mode');
                localStorage.setItem('darkMode', 'disabled');
            }
        });
        
        // Animate progress bars
        function animateProgressBars() {
            const progressBars = document.querySelectorAll('.progress-bar');
            progressBars.forEach(bar => {
                bar.style.width = '100%';
            });
        }
        
        // Animate elements when they come into view
        function animateOnScroll() {
            const elements = document.querySelectorAll('section');
            elements.forEach(element => {
                const elementPosition = element.getBoundingClientRect().top;
                const screenPosition = window.innerHeight / 1.3;
                
                if (elementPosition < screenPosition) {
                    element.style.opacity = '1';
                    element.style.transform = 'translateY(0)';
                }
            });
        }
        
        // Set initial state for animation
        document.querySelectorAll('section').forEach(section => {
            section.style.opacity = '0';
            section.style.transform = 'translateY(20px)';
            section.style.transition = 'opacity 0.6s ease, transform 0.6s ease';
        });
        
        // Profile picture hover effect
        const profilePic = document.getElementById('profile-pic');
        profilePic.addEventListener('mouseenter', () => {
            profilePic.style.transform = 'scale(1.05) rotate(5deg)';
        });
        profilePic.addEventListener('mouseleave', () => {
            profilePic.style.transform = 'scale(1) rotate(0)';
        });
        
        // Initialize animations
        window.addEventListener('load', () => {
            animateProgressBars();
            animateOnScroll();
        });
        
        window.addEventListener('scroll', animateOnScroll);
    </script>
</body>
</html>
