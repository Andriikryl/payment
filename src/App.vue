<script setup lang="ts">
import { ToggleGroupItem, ToggleGroupRoot } from 'radix-vue'
import { AspectRatio } from 'radix-vue'
import { ref } from 'vue'
import { Label } from 'radix-vue'

const toggleStateSingle = ref('left')

const toggleGroupItemClasses = 'hover:bg-green3 text-mauve11 data-[state=on]:bg-[#4242b1] data-[state=on]:text-white flex h-[55px] w-[55px] items-center justify-center bg-white text-base leading-4 first:rounded-l last:rounded-r focus:z-10 focus:shadow-[0_0_0_2px] focus:shadow-black focus:outline-none'
</script>

<template>
    <div class="w-full h-[100dvh] flex">
      <div class="bg-[#4242b1] w-full h-full">
        <div class="flex flex-col items-center mt-12">
          <div class="h-[170px]"></div>
          <div class="min-w-[300px]">
            <div>
              <button class="text-[14px] leading-[18px] overflow-ellipsis break-words text-[rgb(255,_255,_255)] flex items-center gap-2">
                <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 24 24"><path fill="currentColor" d="m6.8 13l2.9 2.9q.275.275.275.7t-.275.7t-.7.275t-.7-.275l-4.6-4.6q-.15-.15-.213-.325T3.426 12t.063-.375t.212-.325l4.6-4.6q.275-.275.7-.275t.7.275t.275.7t-.275.7L6.8 11H20q.425 0 .713.288T21 12t-.288.713T20 13z"/></svg>
                <span>
                  Beck to home
                </span>
              </button>
            </div>
            <div class="h-[10px]"></div>
            <h1 class="text-[16px] leading-[20px] text-[rgba(255,_255,_255,_0.6)]">Subscribe to Arcanum Basic</h1>
            <div class="flex items-center gap-3">
              <p class="text-[36px] leading-[46px] tracking-[-0.48px] text-[rgb(255,_255,_255)]">$296.00</p>
              <span class="text-[16px] leading-[20px] text-[rgba(255,_255,_255,_0.6)]">per <br>
                year</span>
            </div>
            <div class="h-[20px]"></div>
            <div class="flex justify-between items-center">
              <p class="text-[14px] leading-[18px] overflow-ellipsis break-words text-[rgb(255,_255,_255)]">Arcanum Basic</p>
              <p class="text-[14px] leading-[18px] overflow-ellipsis break-words text-[rgb(255,_255,_255)]">$296.00</p>
            </div>
            <div class="h-[10px]"></div>
            <div class="w-full h-[2px] bg-[rgba(255,_255,_255,_0.1)]"></div>
            <div class="h-[50px]"></div>
            <div class="flex justify-between items-center">
              <p class="text-[14px] leading-[18px] overflow-ellipsis break-words text-[rgb(255,_255,_255)]">Subtotal</p>
              <p class="text-[17px] leading-[18px] overflow-ellipsis break-words text-[rgb(255,_255,_255)]">$296.00</p>
            </div>
            <div class="h-[10px]"></div>
            <div class="w-full h-[2px] bg-[rgba(255,_255,_255,_0.1)]"></div>
            <div class="h-[30px]"></div>
            <div class="flex justify-between items-center">
              <p class="text-[14px] leading-[18px] overflow-ellipsis break-words text-[rgb(255,_255,_255)]">Tax</p>
              <p class="text-[17px] leading-[18px] overflow-ellipsis break-words text-[rgb(255,_255,_255)]">Enter address to calculate
              </p>
            </div>
            <div class="h-[10px]"></div>
            <div class="w-full h-[2px] bg-[rgba(255,_255,_255,_0.1)]"></div>
            <div class="h-[40px]"></div>
            <div class="flex justify-between items-center">
              <p class="text-[14px] leading-[18px] overflow-ellipsis break-words text-[rgb(255,_255,_255)]">Total due today</p>
              <p class="text-[21px] leading-[18px] overflow-ellipsis break-words text-[rgb(255,_255,_255)]">$296.00</p>
            </div>
            <div class="h-[10px]"></div>
            <div class="w-full h-[2px] bg-[rgba(255,_255,_255,_0.1)]"></div>
          </div>
        </div>
      </div>
      <div class="bg-[#FFF] w-full h-full">
        <div class="flex flex-col items-center mt-12">
          <div class="h-[170px]"></div>
          <div class="min-w-[300px]">
            <h1 class="text-[16px] leading-[20px] text-[rgba(26,26,26,0.7)]">To pay for your order, 
              <a href="#" class="text-[#4242b1]">
                authorize.
              </a>
            </h1>
            <div class="h-[20px]"></div>
            <div>
              <h1 class="text-[20px] leading-[20px] text-[rgba(26,26,26,0.7)]">
                Currency
            </h1>
            <div class="h-[20px]"></div>
            <div>
              <div>
            <ToggleGroupRoot
              v-model="toggleStateSingle"
              type="single"
              class="flex"
            >
              <ToggleGroupItem
                value="one"
                aria-label="Toggle italic"
                :class="toggleGroupItemClasses"
                class=" border border-[] p-3 text-[20px]"

              >
              KZT
              </ToggleGroupItem>
              <ToggleGroupItem
                value="two"
                aria-label="Toggle italic"
                :class="toggleGroupItemClasses"
                class=" border border-[] p-3 text-[20px]"
              >
              MXN
              </ToggleGroupItem>
              <ToggleGroupItem
                value="three"
                aria-label="Toggle italic"
                :class="toggleGroupItemClasses"
                class=" border border-[] p-3 text-[20px]"
              >
              EUR
              </ToggleGroupItem>
              <ToggleGroupItem
                value="four"
                aria-label="Toggle italic"
                :class="toggleGroupItemClasses"
                class=" border border-[] p-3 text-[20px]"
              >
              USD
              </ToggleGroupItem>
              <ToggleGroupItem
                value="five"
                aria-label="Toggle italic"
                :class="toggleGroupItemClasses"
                class=" border border-[] p-3 text-[20px]"
              >
              UAH
              </ToggleGroupItem>
              <ToggleGroupItem
                value="sixe"
                aria-label="Toggle italic"
                :class="toggleGroupItemClasses"
                class=" border border-[] p-3 text-[20px]"
              >
              RUB
              </ToggleGroupItem>
            </ToggleGroupRoot>
            <br>
          </div>
            </div>
            <div>
              <div class="flex flex-wrap items-baseline justify-between gap-[15px]">
                <Label
                  class="text-[20px] leading-[20px] text-[rgba(26,26,26,0.7)]"
                  for="firstName"
                > Promo code</Label>
                <input
                  id="firstName"
                  class=" shadow-black inline-flex h-[35px] w-[200px] appearance-none items-center justify-center rounded-[4px] px-[10px] text-[15px] leading-none text-[rgba(26,26,26,0.7)] shadow-[0_0_0_1px] outline-none focus:shadow-[0_0_0_2px_black] selection:color-white selection:bg-blackA9 border-[#4242b1]"
                  type="text"
                  value="tipe hier"
                >
              </div>
            </div>
            <div class="h-[40px]"></div>
            <h1 class="text-[20px] leading-[20px] text-[rgba(26,26,26,0.7)]">
              Choose payment method
            </h1>
            <div class="h-[20px]"></div>
            <div class="flex flex-wrap gap-3">
              <div class="shadow-black w-full sm:w-[250px] overflow-hidden rounded-md shadow-[0_2px_10px]">
                <a href="#">
                  <AspectRatio :ratio="16 / 9">
                    <img
                      class="h-full w-full object-cover"
                      src="https://images.unsplash.com/photo-1535025183041-0991a977e25b?w=300&dpr=2&q=80"
                      alt="Landscape photograph by Tobias Tullius"
                    >
                  </AspectRatio>
                </a>
                </div>
              <div class="shadow-black w-full sm:w-[250px] overflow-hidden rounded-md shadow-[0_2px_10px]">
                <a href="#">
                  <AspectRatio :ratio="16 / 9">
                    <img
                      class="h-full w-full object-cover"
                      src="https://images.unsplash.com/photo-1535025183041-0991a977e25b?w=300&dpr=2&q=80"
                      alt="Landscape photograph by Tobias Tullius"
                    >
                  </AspectRatio>
                </a>
                </div>
            </div>
            </div>
            </div>
        </div>
      </div>
    </div>
</template>

<style scoped>

</style>
