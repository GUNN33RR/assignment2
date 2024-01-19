<script setup>
const supabase = useSupabaseClient();
const email = ref("");
const password = ref(null);

async signup(){

  const { data } = await supabase.auth.signUp({

email: email.value,
password: password.value,

//options: { emai

//}



  })
}
</script>

<template>
<main>
<h1>Sign up</h1>
</main>
</template>