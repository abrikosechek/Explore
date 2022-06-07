<template>
  <div class="tickets_page container">
    <div class="pages">
      <button
        :class="{ active: active_link == 0 }"
        class="pages_link"
        @click="change_active_link(0)"
      >
        <img src="../assets/hotel.svg" />
        <p>Hotel</p>
      </button>
      <button
        :class="{ active: active_link == 1 }"
        class="pages_link"
        @click="change_active_link(1)"
      >
        <img src="../assets/Flight.svg" />
        <p>flight</p>
      </button>
      <button
        :class="{ active: active_link == 2 }"
        class="pages_link"
        @click="change_active_link(2)"
      >
        <img src="../assets/car.svg" />
        <p>car</p>
      </button>
      <button
        :class="{ active: active_link == 3 }"
        class="pages_link"
        @click="change_active_link(3)"
      >
        <img src="../assets/Ship.svg" />
        <p>ship</p>
      </button>
    </div>
    <div class="page">
      <div class="forms">
        <div class="forms_comp">
          <p>Your destination</p>
          <input placeholder="Thailand" type="text" />
        </div>
        <div class="forms_comp">
          <p>check in</p>
          <input placeholder="01-26-22" type="text" />
        </div>
        <div class="forms_comp">
          <p>check out</p>
          <input placeholder="01-30-22" type="text" />
        </div>
        <div class="forms_comp">
          <p>child</p>
          <input placeholder="2" type="text" />
        </div>
        <div class="forms_comp">
          <p>adult</p>
          <input placeholder="3" type="text" />
        </div>
        <div class="forms_comp">
          <p>A</p>
          <button>Book now</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "tickets_page",
  data() {
    return {
      active_link: 0,
    };
  },
  methods: {
    change_active_link(num) {
      this.active_link = num;
    },
  },
};
</script>

<style lang="scss">
.tickets_page {
  .pages {
    display: flex;
    flex-direction: row;
    gap: 10px;

    .pages_link {
      display: flex;
      align-items: center;
      justify-content: flex-start;
      gap: 10px;
      min-width: 120px;
      height: 40px;
      padding: 0 15px;
      border-radius: 4px 4px 0 0;
      background-color: white;
      box-shadow: 0 0 5px rgba(0, 0, 0, 0.1);
      & > img {
        width: 25px;
        height: 25px;
      }
      & > p {
        font-weight: 500;
        font-size: 16px;
        text-transform: capitalize;
      }
      &.active {
        background-color: #ffc814;
      }
    }
  }

  .page {
    padding: 25px 15px 20px;
    width: 100%;
    background-color: white;
    border-radius: 0 0 4px 4px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);

    .forms {
      display: grid;
      grid-template-columns: repeat(6, 1fr);
      gap: 50px;

      .forms_comp {
        p {
          font-weight: 600px;
          font-size: 16px;
          text-transform: capitalize;
          color: #1f3347;
        }
        input {
          padding: 0 10px;
          margin-top: 10px;
          width: 100%;
          height: 40px;
          background-color: white;
          border: none;
          border-radius: 4px;
          box-shadow: 2px 2px 6px rgba(0, 0, 0, 0.2);
        }

        &:last-child {
          p {
            font-weight: 600px;
            font-size: 16px;
            text-transform: capitalize;
            color: white;
          }
          button {
            width: 100%;
            margin-top: 10px;
            height: 40px;
            background-color: #ffc814;
            border-radius: 4px;
            font-size: 16px;
            box-shadow: 0px 0px 2px rgba(125, 98, 11, 0.4);
          }
        }
      }
    }
  }
}
</style>
