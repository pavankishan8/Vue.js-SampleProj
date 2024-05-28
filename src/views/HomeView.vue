<template>
  <div class="header">
    <div class="leftHead">
      <img alt="Vue logo" class="image" src="@/assets/logo.svg" width="60" height="60" />
      <span class="wording">Vue.Js</span>
    </div>
    <div class="rightHead">
      <button class="rightBtn">
        <img alt="Vue logo" class="image2" src="@/assets/user-image.png" width="30" height="30" />
        <span class="wordings"> Pavan Raj </span>
      </button>
    </div>
  </div>
  <div class="body">
    <div style="width: 100%; display: flex; background-color: rgb(23, 22, 46)">
      <div
        style="
          width: 60%;
          height: 90vh;
          display: flex;
          flex-direction: column;
          justify-content: center;
          align-items: flex-start;
        "
      >
        <span
          id="hello-text"
          style="
            margin-left: 5%;
            color: white;
            font-weight: 500;
            opacity: 0;
            transform: translateY(-50px);
            transition:
              opacity 0.3s,
              transform 0.3s;
          "
          >Hello, It's me</span
        >
        <p
          id="name-text"
          style="
            font-size: 28px;
            margin-left: 5%;
            color: white;
            font-weight: 500;
            opacity: 0;
            transform: translateX(-50px);
            transition:
              opacity 0.3s,
              transform 0.3s;
          "
        >
          Pavan Kishan
        </p>
        <span
          id="prof-text"
          style="
            margin-left: 5%;
            color: white;
            font-weight: 500;
            opacity: 0;
            transform: translateY(-50px);
            transition:
              opacity 0.3s,
              transform 0.3s;
          "
          >and I'm a <span style="color: blue; font-weight: 500">Photographer</span></span
        >
        <br />
        <p
          id="desc-text"
          style="
            margin-left: 5%;
            color: white;
            font-weight: 500;
            opacity: 0;
            transform: translateX(-50px);
            transition:
              opacity 0.3s,
              transform 0.3s;
          "
        >
          See America Through My Eye Behind the lens of some of the most exclusive weddings in the
          USA and worldwide Published on Harper's Bazaar, Vogue, Martha Stewart, Elle...
        </p>
      </div>
    </div>
  </div>
</template>

<style>
@keyframes slideInFromTop {
  0% {
    opacity: 0;
    transform: translateY(-50px);
  }
  100% {
    opacity: 1;
    transform: translateY(0);
  }
}

@keyframes slideInFromLeft {
  0% {
    opacity: 0;
    transform: translateX(-50px);
  }
  100% {
    opacity: 1;
    transform: translateX(0);
  }
}

@keyframes slideInFromBottom {
  0% {
    opacity: 0;
    transform: translateY(50px);
  }
  100% {
    opacity: 1;
    transform: translateY(0);
  }
}

@keyframes slideInFromRight {
  0% {
    opacity: 0;
    transform: translateX(50px);
  }
  100% {
    opacity: 1;
    transform: translateX(0);
  }
}

#hello-text {
  animation: slideInFromTop 0.3s ease-out 0.3s forwards;
}

#name-text {
  animation: slideInFromLeft 0.3s ease-out 0.3s forwards;
}

#prof-text {
  animation: slideInFromBottom 0.3s ease-out 0.3s forwards;
}

#desc-text {
  animation: slideInFromRight 0.3s ease-out 0.3s forwards;
}

#more-btn {
  animation: slideInFromRight 0.3s ease-out 0.5s forwards;
}

@keyframes rollInFromRight {
  0% {
    opacity: 0;
    transform: translateX(50px);
  }
  100% {
    opacity: 1;
    transform: translateX(0);
  }
}

#facebook-icon {
  animation: rollInFromRight 0.3s ease-out 0.3s forwards;
}

#whatsapp-icon {
  animation: rollInFromRight 0.3s ease-out 0.4s forwards;
}

#instagram-icon {
  animation: rollInFromRight 0.3s ease-out 0.5s forwards;
}

#linkedin-icon {
  animation: rollInFromRight 0.3s ease-out 0.6s forwards;
}

@keyframes fadeIn {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}

#fade-in-image {
  animation: fadeIn 0.5s ease-out 0.5s forwards;
}

.header {
  background-color: rgb(15, 161, 245);
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.rightBtn {
  display: flex;
  align-items: center;
  gap: 6px;
  background: none;
  outline: none;
  border: none;
}

.rightBtn:hover {
  padding: 5px;
  background-color: #3db68c;
}

.rightHead {
  display: flex;
  align-items: center;
  margin-right: 1%;
  gap: 6px;
}

.leftHead {
  display: flex;
  align-items: center;
}

.image {
  padding: 5px;
}

.image2 {
  padding: 5px;
  background-color: white;
}

.wordings {
  font-weight: 700;
  color: white;
}

.wording {
  color: white;
  font-weight: 700;
}
</style>
