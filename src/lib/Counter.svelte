<script lang="ts">
  const btn_calculate = document.getElementById('btn_calculate')
    const input_weight = document.getElementById('weight')
    const input_height = document.getElementById('height')
    const result = document.getElementById('result')
    const bmi_span = document.getElementById('bmi')
</script>

<button btn_calculate.onclick>
  (event) => {event.preventDefault()
  const weight = Number(input_weight.value)
  const height = Number(input_height.value)
  const bmi = weight / (height*height)
  bmi_span.innerHTML = bmi.toFixed(1)
  result.style.display = 'flex'
  result.classList.add('visivel')
  result.classList.remove('visivel')
</button>

