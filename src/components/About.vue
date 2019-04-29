<template>
  <div>
    <h1>About</h1>
    <p>
      Hi team, although a front end for the project was not specified, I took the liberty of putting together a short taster.
      In the front end you can see an example of how the back end of the app you requested could feed into a GUI instead of the user manually messing about with different endpoints.
    </p>

    <h6>As for the back end please find a list below of the different endpoints and details of what data they return.</h6>
    <h6>
      <strong>Legend: http://localhost:8080/Fuels/(month)/(driver id)/details/fueltype</strong>
    </h6>
    <ul>
      <li>
        <strong>Filtered by month, driver id, fuel type -</strong>//localhost:8080/Fuels/1/5/details/fueltype
      </li>
      <li>
        <strong>Filtered by month, driver id -</strong>http://localhost:8080/Fuels/1/5/
      </li>
      <li>
        <strong>Filtered by month -</strong>http://localhost:8080/Fuels/1/details
      </li>
      <li>
        <strong>Filtered by month, driver id-</strong>http://localhost:8080/Fuels/1/5/details
      </li>
      <li>
        <strong>Filtered by month, driver id, total cost, fuel type -</strong>http://localhost:8080/Fuels/1/details/fueltype
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "About" //this is the name of the component
};
</script>
<style>
li {
  margin: 20px;
}
</style>
