<script lang="ts">
type Props = {
  case:string
}
export default{
  props:{
    case:String
  },
  setup(props:Props,{ slots }:any){
    return ()=>{
      //判断是否有case,有则返回插槽里显示的
      if(slots[props.case]){
        return slots[props.case]()
      }

      //当没有case的时候，展示default
      if(slots.default){
        return slots.default()
      }
    }
  } 
}

</script>
<template>
  <div>
  </div>
</template>