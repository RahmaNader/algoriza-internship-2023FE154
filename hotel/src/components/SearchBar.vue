<template>
    <div class="search-bar">
        <div class="location-picker">
            <img class="location-icon" src="../assets/location1.png" alt="Location Icon" />
            <p class="location-text">Where are you going?</p>
            <img class="dropdown-icon" src="../assets/arrow-down1.png" alt="Dropdown Icon">
        </div>
        <div class="date-picker">
            <img class="calendar-icon" src="../assets/calendar1.png" alt="Calendar Icon" />
            <p class="date-text">Check in date</p>
        </div>
        <div class="date-picker1">
            <img class="calendar-icon" src="../assets/calendar1.png" alt="Calendar Icon" />
            <p class="date-text">Check out date</p>
        </div>
        <div class="guests">
            <img class="guests-icon" src="../assets/guests.png" alt="Guests Icon" />
            <p class="guests-text">Guests</p>
        </div>
        <div class="rooms">
            <img class="rooms-icon" src="../assets/rooms.png" alt="Rooms Icon" />
            <p class="rooms-text">Rooms</p>
        </div>
        <div class="search-button">
            <button class="search-button">Search</button>
        </div>
    </div>
</template>

<script>
export default {
    name: 'SearchBar',
}
</script>

<style scoped>
.search-bar {
  position: absolute;
  width: 1100px;
  height: 64px;
  left: 10%;
  top: 548px;
  background: #FFFFFF;
  box-shadow: 0px 4px 37px rgba(0, 0, 0, 0.15);
  border-radius: 8px;
  display: flex; /* Add this line */
  justify-content: space-evenly; /* Add this line */
  align-items: center; /* Add this line */
    padding: 0 20px;
}

.location-picker, .date-picker, .date-picker1, .guests, .rooms {
  width: 250px;
  height: 43px;
  background: #F2F2F2;
  border-radius: 4px;
  display: flex;
  align-items: center;
  margin: 10px;
}

.location-picker .location-icon, .date-picker .calendar-icon, .date-picker1 .calendar-icon, .guests .guests-icon, .rooms .rooms-icon {
  width: 20px;
  height: 20px;
  flex: none;
  order: 0;
  flex-grow: 0;
    margin: 0 5px;
}

.location-picker .location-text, .date-picker .date-text, .date-picker1 .date-text, .guests .guests-text, .rooms .rooms-text {
  flex: none;
  order: 1;
  flex-grow: 0;
}

.location-picker .dropdown-icon {
  width: 20px;
  height: 20px;
  flex: none;
  order: 2;
  flex-grow: 0;
  cursor: pointer;
}

.search-button {
    width: 100px;
    height: 43px;
    background: #2F80ED;
    border-radius: 6px;
    border: none;
    font-style: normal;
    font-weight: 500;
    font-size: 20px;
    line-height: 20px;
    /* identical to box height, or 133% */
    letter-spacing: 0.02em;
    color: #FFFFFF;
    cursor: pointer;
}
</style>
