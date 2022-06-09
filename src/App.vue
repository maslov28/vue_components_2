<template>
  <ul>
    <li>создать два SFC BaseCard.vue и BaseCards.vue</li>
    <li>Структура компонентов
      <ul>
        <li>App.vue
          <ul>
            <li>BaseCards (принимает параметров массив [{id: 1, title: ‘Card1’}, {id: 2, title: ‘Card2’}]) и рендерит в цикле BaseCard
              <ul>
                <li>
                  BaseCard (принимает параметром title и рендерит его)
                </li>
              </ul>
            </li>
          </ul>
        </li>
      </ul>
    </li>
  </ul>

  <base-cards
    :array="array"
  ></base-cards>

</template>

<script>
import BaseCards from './components/BaseCards.vue'
export default {
  components: {BaseCards},
  data() {
    return {
        array: [
          {id: 1, title: 'Card1'}, 
          {id: 2, title: 'Card2'}
        ]
    }
  }
}
</script>