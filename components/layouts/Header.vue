<template>
  <div class="border-b-2">
    <header class="container mx-auto items-center h-20 grid gap-3 grid-cols-4 justify-around">
    <div><img class="h-10 align-middle" src="/images/logo.png" alt="Logo" /></div>
    <div class="grid grid-cols-5  col-span-2">
      <LayoutsNavLink  to="/" text="Docs" />
      <LayoutsNavLink to="/" text="Modules" />
      <LayoutsNavLink to="/" text="Showcase" />
      <LayoutsNavLink to="/" text="Support" />
      <LayoutsNavLink to="/" text="Blog" />
    </div>
    <div><input type="text" placeholder="Search"/></div>
  </header>
</div>

</template>
