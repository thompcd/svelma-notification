<script>
import 'bulma/css/bulma.css'
import { Button, Notification } from 'svelma'

  function showNotification(props) {
    Notification.create({
      message: 'You opened this programmatically!',
      ...props
    })
  }
</script>
<!-- <div style="width:100% !important; height:100% !important;"> -->
<div style="width:100px !important; height:100px !important;">
	<Button class="block" type="is-danger" on:click={() => showNotification({ type: 'is-danger', position: 'is-top-right', icon: true })}>Show Notification (danger)</Button>
</div>
