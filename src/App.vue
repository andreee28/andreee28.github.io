<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
</script>

<template>
  <header>
    <img alt="Vue logo" class="logo" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAL0AAAELCAMAAAC77XfeAAAAhFBMVEX+/v4CAgIAAAD8/Pz5+fkFBQX29vbw8PDm5ubz8/OxsbHZ2dm5ubnLy8vr6+upqalAQEARERHFxcU2NjZeXl7T09OOjo6Hh4fg4OBxcXGhoaGRkZE5OTkdHR2+vr6YmJhWVlZra2svLy98fHxJSUlcXFxLS0smJiYWFhaAgIAjIyNtbW1oA5u7AAAHiklEQVR4nO2ciZKqOhCGY4KyLyKL4iiKjsuZ93+/m7CGzcG5qKGqv1M15QETfpuk02kSEAIAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAQiRCESPaZPFuY1P9wJ8gfanseYvl7LQqCMIxtc/Fsad0ON5swjiPD4g9LlrnfK+OJ7ICs94F3xTUuW0MdWn6xsB2u6MFmcglSIi/Jjjjaq6y/1rxbdo0ZR3rA04ZVod240mnJ68HbHIpa5/SYsx5bNyGSHict4fwvuGnkF6tJaLFplS/uAndgN/hODkSNVr3KSxWH3xqtvnpYRVmVO7J677H0Qv++32UQCWmDtNOKopHVXwddFz+6rhT2tprGcXwcV7w81Gp422d9lfbMOffVOVOdHEM7OjEnxJ/CyW896DmUUj3uhJN/765hfeUFpoU2royyEUqJvuqVWN2V/BG9Er9becfTKdgG983RO5+dZFa/9TjoMpy+5G8enuNlJJUn2SfzwsvXpXYV/0f9PBff7peSaoYz3ocrbfXrZWOEODWcIlWrLasbbIwpHq3zevFV4iIRksI+yVyPxH6ruPRVF780m/EMq0b2iuZPe8+YKIX6Vfd5gtyy+WCzdTKuiz93N2sJ2Xkl+DSqerVQdusJyQiynD71klrzWPhEpE6XQu2/zoYz7I2qHu1w0ah7v7I44x7bx3X1j5oFSZtg3y3+K06hXs8u0mU8P7Nbu91f6+qx1+4ZWaWsWveGacd4Oup+yCZXvyomFZKs+IYdxSzGD0LbXS/svM22nPWCOsi6x8H/NrGtabR4GN5DQ6P/XN3KLaJQ378aN0q2WfRKh8fMlSlh0hqwCn+Hl1LDWcu1gZQx7xzykrvC7I/UK9bGtb2VXSBAVJpyLEbYykvOKpfjNUcEuWH7vEQ5RmSjXTb8Wszz68dRBytqEl2LbNdCRE1947xpTU5Wa5rSqb4LNjWx005FxpVf/gwUPQ7YOrySjPmRFrfaUb34/ZXT8v0vhsSHVhGVK0Ibx6o7LC6/MO5IVUPhAxrOikVjwh0hCvnHFXKQGiyZ9vl33Y0W1WEcote0G4S2fKRcNQhc+iCn48oHLnq80P9Liq7rC37OgA3XCM9F9x17YlhyKf3ERUNx5TXuyNfC7/P53hXC3DmZ3Dh0rmLKZXogD/MxHntWnkOKEWm1pyZc7Er1+qPEmsFPPOTiqKQUYzDOggfqapCZ5kbGntfm0vxcfF69mV1+/ngiShS+jXBRgnzKm9sxvyHsp/vftPm9Rv0e55mPPGAwsu72pT7uZw7fwvkTenBwnNCtuilz9PrJfk02U2dabe6Aam+cc0R+uZpWeae+ee8boMa+xwovlXB/+5FrLvNTDNPagceNEuobctzj4nLG339azLMQsipb/msDmddQpTBx8qo44FUQIu2qcVmfnvGrmTmOP63leeRdqd55x5O1UeEyUp2pQsEhpIin5zRKmpx8ZJf99vJpKc9D0FeZiB43Pf8OaOxejFi1OG8iLNCpaDqHT2v5C9RrzotIbXr9tpiL0SlKdw5ccLb5vHjkR5pvgmTJETyTp2h7Ii+zHP+4j9XehJQ3fXz+tJI/omXGH/eJ7LuQUJCm+44TjHUY5Aezhyf6p3X8DWnBMgxjP9R8HwvmN1+XKX4xRPLwHO/GfbL2Nggi31R+PM1+y2ZaG/zoubvgEGTg6WXVSghS/Km2HIY00fFqelR2npTNedloIUv1Y8Ij60YchkHs+vEF49uXF5sveqI5KtTMqrbh16uXeLbSvUJJHIgcLjvXI6TLcy6CT6+spG8pRTo/wStT5A6g1da1tH4HvQMiZ/Ij3Fy1XFuZw87G4lpf32G8PVET/3Mu3ubn4LRW5bxwOcj/h5g+WzxY+kfJL1e0sdU8zPhXgYP8tlO0jMCr+dApRslEVdZrXXcNd5KJkRJhe+0gpq0eAAAAAIBRqAUEUvuQyMj+mtdqmYZhTCEtQkX7cRrQf53SXWSK7RU7fpzYEv0OrB2cbyLDeBUcd9XskH04iTu1Yma1cW2rR31eS2/CUtysjqWtHu3wybZpHAVbKCUh43Q4HLxVOv3uFV/8hKUhVE6QfD/ck9SSj39EUh/iWbUNb9AP2AmUEzw8IbywfyhMbuHnGbsX8r9lQcy/7RNf+PnOc8nob275G26PvmZKtpGUXYrReBrvHyhkzy+B7bo+xdxHm9YrYQRZ80L4vW1pTDNz7rbZXPhtGU72up/ym4I0HXTDpc2/7kbvIi7/wG+Cu71V4gPyRPf1pLEwgPQ8YGMb+MttogI9SPH/0YByO2ThnJUPDnOciBPvS7JMhjwUJ+WrDoRp9cORUPkShoGv/BIIwrZPZupDQUbaobC9qHEx72q9g0FwpLVrfxdzREeUIKcP87T58Tw6aTlcnCS58RMA/CXu7DZDakY5s8rR/yyI6PL3uyqXUA9vJrGFRo2SemCWrQNImu8KEhYzSJoNSJjwYBCWG92Pq+tumVw2seaL7mtqTEgqAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAHyW/wCnIUz70L8BywAAAABJRU5ErkJggg==" width="140" height="140" />

    <div class="wrapper">
      <HelloWorld msg="OWI!" />
    </div>
  </header>

  <main>
    <TheWelcome />
  </main>
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
