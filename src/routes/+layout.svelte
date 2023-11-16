<script>
  import "$lib/style/app.css";
  const year = new Date().getFullYear();
</script>

<nav>
  <ul>
    <li>
      <a href="/contact">ادعم فلسطين</a>
    </li>
    <li>
      <a href="/">الرئيسية</a>
    </li>
  </ul>
</nav>

<main>
  <slot />
</main>

<footer>
  <p>تم التصميم بواسطة محمد ياسر. {year}</p>
</footer>

<style lang="scss">
  main {
    display: flex;
    justify-content: center;
    align-items: center;
  }

  ul {
    list-style: none;
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: #000;

    li {
      padding: 1rem;
      user-select: none;
    }

    a {
      text-decoration: none;
      color: white;
      font-size: 1rem;
    }
  }

  footer {
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 0.5rem;
    color: green;
    user-select: none;
    // background-color: green;
  }
</style>
