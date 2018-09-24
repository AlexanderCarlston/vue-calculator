<template>
    <div id="calculator">
      <div id="screen-container">
        <div id="screen"></div>
      </div>

      <div id="buttons-container">
        <div class="buttons">
          <span class="operator" id="clear">C</span>
          <span class="operator">/</span>
          <span class="operator">*</span>
          <span>7</span>
          <span>8</span>
          <span>9</span>
          <span class="operator">-</span>
          <span>4</span>
          <span>5</span>
          <span>6</span>
          <span class="operator">+</span>
          <span>1</span>
          <span>2</span>
          <span>3</span>
          <span class="operator" id="equals">=</span>
          <div class="l-row">
            <span id="zero">0</span>
          </div>
        </div>
      </div>
    </div>
</template>
<script>
export default {
    name: "Calculator"
}
</script>
<style>
#calculator {
  background: #2B3D50;
  border-radius: 20px;
  padding: 15px;
  width: 335px;
  margin-left: auto;
  margin-right: auto;
}

#screen-container {
  background: #5E626D;
  border-radius: 10px;
  padding: 20px;
}

#screen {
  background: #EF5D5D;
  border: none;
  font-family: 'Orbitron', sans-serif;
  font-size: 1.4em;
  font-weight: 600;
  height: 23px;
  overflow: hidden;
  padding: 12px 15px;
  width: 265px;
  z-index: 1;
}

#zero {
  width: 225px;
}

#clear {
  background: #CF7C43;
  width: 147px;
}

#clear:active {
  background-color: #E67E22;
}

#equals {
  height: 89px;
}

#buttons-container {
  padding: 30px 0 0 15px;
}

.l-row {
  position: absolute;
  top: 354px;
}

.buttons {
  overflow: hidden;
}

.buttons span {
  background: #3383D2;
  border-radius: 3px;
  border: none;
  box-shadow: inset 0px 1px 0px #5E626D, 0px 5px 0px 0px #45637F;
  cursor: pointer;
  float: left;
  font-family: 'Oswald', sans-serif;
  width: 70px;
  height: 40px;
  margin: 0 7px 11px 0;
  line-height: 40px;
  text-align: center;
}

.buttons span:active {
  background-color: #4AA3DF;
  top: 3px;
  box-shadow: inset 0px 1px 0px #5E626D, 0px 2px 0px 0px #45637F;
}

.operator {
  font-size: 1.3em;
}
</style>
