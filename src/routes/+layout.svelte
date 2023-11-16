<script>
  import "$lib/style/app.css";
  const year = new Date().getFullYear();
</script>

<svelte:head>
  <title>الحب: الرئيسية</title>
</svelte:head>

<nav>
  <ul>
    <li>
      <a class="support" href="/contact">ادعم فلسطين</a>
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
  <p>🇵🇸 تم التصميم بواسطة محمد ياسر. {year} 🇵🇸</p>
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

    a.support {
      text-decoration: underline;
      text-decoration-color: red;
      // text-decoration-thickness: 6px;
      text-decoration-style: double;
    }
  }

  footer {
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 0.5rem;
    color: white;
    user-select: none;
    // background-color: black;
  }
</style>
