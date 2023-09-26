<template>
  <div id="app">
    <!-- Header -->
    <header>
      <h1>Anjali Chahar</h1>
      <nav>
        <ul>
          <li><router-link to="/about">About</router-link></li>
          <li><router-link to="/projects">Projects</router-link></li>
          <li><router-link to="/contact">Contact</router-link></li>
        </ul>
      </nav>
    </header>

    <!-- Main Content -->
    <main>
      <router-view></router-view>
    </main>

    <!-- Footer -->
    <footer>
      <p>&copy; 2023 AC</p>
    </footer>
  </div>
</template>

<script>
export default {
  name: 'App'
};
</script>

<style>
/* Your global CSS styles here */
body {
  font-family: Arial, sans-serif;
  background-color: #f0f0f0;
  color: #333;
  line-height: 1.6;
  margin: 0;
  padding: 0;
}

/* Style the header section */
header {
  background-color: #007acc;
  color: #fff;
  text-align: center;
  padding: 1rem 0;
}

/* Style the navigation menu */
nav ul {
  list-style: none;
}

nav ul li {
  display: inline;
  margin-right: 20px;
}

nav a {
  text-decoration: none;
  color: #fff;
  font-weight: bold;
}

/* Style the individual sections */
section {
  margin-bottom: 40px;
}

/* Style headings and paragraphs */
h2, h3 {
  color: #007acc;
}

/* Style the contact form */
form {
  background-color: #fff;
  padding: 20px;
  border-radius: 5px;
  box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
}

label {
  display: block;
  margin-bottom: 10px;
}

input[type="text"],
input[type="email"],
textarea {
  width: 100%;
  padding: 10px;
  margin-bottom: 15px;
  border: 1px solid #ccc;
  border-radius: 5px;
}

button[type="submit"] {
  background-color: #007acc;
  color: #fff;
  padding: 10px 20px;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}

button[type="submit"]:hover {
  background-color: #005c99;
}
</style>
