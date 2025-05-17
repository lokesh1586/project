# Project Responsive Web Design using Bootstrap
# Date:
# AIM:
To create a simplified clone of Dribbble (https://dribbble.com/) landing page.

# DESIGN STEPS:
## Step 1:
Clone the repository from GitHub.

## Step 2:
Create Django Admin project.

## Step 3:
Create a New App under the Django Admin project.

## Step 4:
Insert the necessary CSS and JavaScript files as external in order to use Bootstrap.

## Step 5:
Create a HTML file and include the needed Bootstrap components.

## Step 6:
Publish the website in the LocalHost.

# PROGRAM :
```

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dribbble</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>
    <nav class="navbar navbar-expand-lg navbar-light bg-white shadow-sm">
        <div class="container">
            <a class="navbar-brand" href="#"><img src="logo.jpg" alt="Logo" class="img-fluid" style="height: 40px;"></a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav me-auto">
                    <li class="nav-item"><a class="nav-link text-dark" href="#">Explore</a></li>
                    <li class="nav-item"><a class="nav-link text-dark" href="#">Hire a Designer</a></li>
                    <li class="nav-item"><a class="nav-link text-dark" href="#">Find Jobs</a></li>
                    <li class="nav-item"><a class="nav-link text-dark" href="#">Blog</a></li>
                </ul>
                <div class="d-flex">
                    <button class="btn btn-dark me-2" data-bs-toggle="modal" data-bs-target="#loginModal">Login</button>
                    <button class="btn btn-outline-dark" data-bs-toggle="modal" data-bs-target="#signupModal">Sign Up</button>
                </div>
            </div>
        </div>
    </nav>

    <div class="modal fade" id="loginModal" tabindex="-1" aria-labelledby="loginModalLabel" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header">
                    <h5 class="modal-title" id="loginModalLabel">Login</h5>
                    <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                </div>
                <div class="modal-body">
                    <form>
                        <div class="mb-3">
                            <label for="loginUserId" class="form-label">User ID</label>
                            <input type="text" class="form-control" id="loginUserId" placeholder="Enter your user ID">
                        </div>
                        <div class="mb-3">
                            <label for="loginPassword" class="form-label">Password</label>
                            <input type="password" class="form-control" id="loginPassword" placeholder="Enter your password">
                        </div>
                        <button type="submit" class="btn btn-dark w-100">Login</button>
                    </form>
                </div>
            </div>
        </div>
    </div>

    <div class="modal fade" id="signupModal" tabindex="-1" aria-labelledby="signupModalLabel" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header">
                    <h5 class="modal-title" id="signupModalLabel">Sign Up</h5>
                    <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                </div>
                <div class="modal-body">
                    <form>
                        <div class="mb-3">
                            <label for="signupName" class="form-label">Full Name</label>
                            <input type="text" class="form-control" id="signupName" placeholder="Enter your full name">
                        </div>
                        <div class="mb-3">
                            <label for="signupAddress" class="form-label">Address</label>
                            <input type="text" class="form-control" id="signupAddress" placeholder="Enter your address">
                        </div>
                        <div class="mb-3">
                            <label for="signupDOB" class="form-label">Date of Birth</label>
                            <input type="date" class="form-control" id="signupDOB">
                        </div>
                        <div class="mb-3">
                            <label for="signupUserId" class="form-label">User ID</label>
                            <input type="text" class="form-control" id="signupUserId" placeholder="Create a user ID">
                        </div>
                        <div class="mb-3">
                            <label for="signupPassword" class="form-label">Password</label>
                            <input type="password" class="form-control" id="signupPassword" placeholder="Create a password">
                        </div>
                        <button type="submit" class="btn btn-dark w-100">Sign Up</button>
                    </form>
                </div>
            </div>
        </div>
    </div>

    <div class="container text-center py-5">
        <h1 class="display-4 fw-bold">Discover the world's top designers</h1>
        <p class="lead text-muted">Explore work from the most talented and accomplished designers ready to take on your next project.</p>
        <div class="input-group my-4">
            <input type="text" class="form-control border-dark text-dark" placeholder="What are you looking for?" style="background-color: white;">
            <button class="btn btn-dark" type="button">Search</button>
        </div>
        <div class="d-flex justify-content-center flex-wrap">
            <span class="badge bg-light text-dark me-2 mb-2">Trending searches:</span>
            <span class="badge bg-secondary me-2 mb-2">Landing Page</span>
            <span class="badge bg-secondary me-2 mb-2">Mobile App</span>
            <span class="badge bg-secondary me-2 mb-2">Logo Design</span>
        </div>
    </div>

    <div class="container py-5">
        <h2 class="mb-4">Popular Projects</h2>
        <div class="row row-cols-1 row-cols-md-3 g-4">
            <div class="col">
                <div class="card border-dark">
                    <img src="1.jpg" class="card-img-top" alt="Project 1">
                    <div class="card-body">
                        <h5 class="card-title">Geometrics</h5>
                        <p class="card-text">A project on geometric designs.</p>
                    </div>
                </div>
            </div>
            <div class="col">
                <div class="card border-dark">
                    <img src="2.jpg" class="card-img-top" alt="Project 2">
                    <div class="card-body">
                        <h5 class="card-title">Low Poly Designs</h5>
                        <p class="card-text">A project on low poly designs.</p>
                    </div>
                </div>
            </div>
            <div class="col">
                <div class="card border-dark">
                    <img src="3.jpg" class="card-img-top" alt="Project 3">
                    <div class="card-body">
                        <h5 class="card-title">Conspiracies</h5>
                        <p class="card-text">A project on Conspiracies.</p>
                    </div>
                </div>
            </div>
            <div class="col">
                <div class="card border-dark">
                    <img src="4.jpg" class="card-img-top" alt="Project 4">
                    <div class="card-body">
                        <h5 class="card-title">Brand Identity</h5>
                        <p class="card-text">A creative take on branding concepts.</p>
                    </div>
                </div>
            </div>
            <div class="col">
                <div class="card border-dark">
                    <img src="5.jpg" class="card-img-top" alt="Project 5">
                    <div class="card-body">
                        <h5 class="card-title">Typography</h5>
                        <p class="card-text">Beautiful typographic layout examples.</p>
                    </div>
                </div>
            </div>
            <div class="col">
                <div class="card border-dark">
                    <img src="6.jpg" class="card-img-top" alt="Project 6">
                    <div class="card-body">
                        <h5 class="card-title">UX/UI Showcase</h5>
                        <p class="card-text">Stunning user experience design samples.</p>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <footer class="bg-dark text-white py-4">
        <div class="container text-center">
            <p>Designed by Dharini</p>
        </div>
    </footer>
</body>
</html>

```
# OUTPUT:
![Screenshot 2025-05-17 075022](https://github.com/user-attachments/assets/20de04ef-e3d4-440e-ba2a-50b6fcb02062)
![Screenshot 2025-05-17 075043](https://github.com/user-attachments/assets/7b06fabe-285e-4944-93ae-74c973a537a9)
![Screenshot 2025-05-17 075101](https://github.com/user-attachments/assets/e666e679-f35f-4914-acdb-5f71a6606a2b)

# RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
