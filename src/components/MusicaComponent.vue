<template>
  <div>
    <div ref="document">
      <div id="element">
        <ul>
          <li>Test 1</li>
          <li>Test 2</li>
          <li>Test 3</li>
          <li>Test 4</li>
          <li>Test 5</li>
          <li>Test 6</li>
        </ul>
      </div>
      <button @click="randomize()">Randomize</button>
    </div>
  </div>
</template>

<script>
import music from './../assets/audio/champions.mp3'
import html2pdf from 'html2pdf.js'

export default {
    name: "MusicaComponent",
    methods: {
      randomize(){
        this.playMusic();
        this.exportToPdf(),{
          filename: "prueba.pdf"
        };
      },

      playMusic(){
        var audio = new Audio(music)
        audio.play()
      },

      exportToPdf() {
        html2pdf(document.getElementById('element'))
      }
    }
}
</script>

<style>

</style>