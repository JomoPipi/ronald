<script>
  import Dropdown from "../Utility/Dropdown.svelte";
</script>

<Dropdown
  title="Crypto Pump Notifier"
  btnImgSrc="images/cryptopumpnotifier.png"
>
  <slot>
    <a target="_blank" href="https://crypto-pump-notifier.vercel.app">
      Crypto Pump Notifier</a
    >
    is a free service that lets you set up email alerts so you can get notified when
    your coins pump. You select the coins and you select the threshold. No need to
    sign up!

    <div>
      <img class="fit" alt="crypto alert success" src="images/cpnalert.png" />
    </div>

    <br />
    Technical challenges:
    <ul>
      <li>
        <b>Email Verification</b><br /> Email verification involves a JWT-secured
        link that confirms their alert when clicked. The link contains data about
        the alert but cannot be altered in any way. Attempting to set up another
        alert when one is already active results in an override confirmation email.
      </li>
      <li>
        <b>Price Fetching and Notifications</b> <br />
        A cronjob fetches the prices of coins using and stores them in the database.
        Users with one or more exceeded thresholds get notified about price changes
        regarding the corresponding coins.
      </li>
    </ul>
  </slot>
</Dropdown>

<style>
  .fit {
    display: absolute;
    display: block;
    height: auto;
    margin-bottom: 1em;
    max-width: 75%;
  }
</style>
