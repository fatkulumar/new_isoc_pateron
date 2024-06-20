<template>
    <div>
        <div class="mt-10 sm:mx-auto sm:w-full sm:max-w-sm">
            <p class="text-3xl">
                Login here!
            </p>
            <form class="pt-6" action="#" method="POST">
                <div>
                    <label for="email" class="block text-sm font-medium leading-6 text-gray-500">Email</label>
                    <div class="mt-2">
                        <input id="email" name="email" placeholder="Enter your Email here!" type="email" autocomplete="email" required
                            class="p-2 block w-full rounded-md border-0 py-3 text-gray-900 shadow-sm ring-1 ring-inset ring-gray-300 placeholder:text-gray-400 focus:ring-2 focus:ring-inset focus:ring-indigo-600 sm:text-sm sm:leading-6">
                    </div>
                </div>

                <div class="pt-4">
                    <div class="flex items-center justify-between">
                        <label for="password" class="block text-sm font-medium leading-6 text-gray-500">Password</label>
                    </div>
                    <div class="flex">
                        <!-- <div class="mt-2"> -->
                            <input id="password" placeholder="Enter your Password here!" name="password" type="password" autocomplete="current-password" required
                                class="p-2 block w-full border-0 py-2 text-gray-900 shadow-sm  placeholder:text-gray-400 focus:ring-2 focus:ring-inset focus:ring-indigo-600 sm:text-sm sm:leading-6 border-y border-l border-gray-400 rounded-l-md">
                        <!-- </div> -->
                        <div class="flex flex-row-reverse items-center cursor-pointer w-1/12">
                            <div class="flex flex-row-reverse border-gray-400 border-y border-r py-2 rounded-r-md">
                                <img width="100%" src="/login/eye-open.svg" alt="">
                            </div>
                        </div>
                    </div>
                </div>
                <div class="flex justify-between py-2">
                    <div class="flex gap-2">
                        <input type="checkbox" name="" id="">
                        <label for="">Rememmber Me</label>
                    </div>
                    <div>
                        <div class="flex items-center justify-between">
                            <div class="text-sm">
                                <a href="#" class="font-semibold text-gray-400 hover:text-indigo-500">Forgot password ?</a>
                            </div>
                        </div>
                    </div>
                </div>

                <div>
                    <button type="submit"
                        class="flex w-full justify-center rounded-md bg-green-500 px-3 py-3 text-md font-semibold leading-6 text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600">
                        Login
                    </button>
                </div>
            </form>

            <p class="text-sm text-gray-500 pt-1">
                Don't have account yet?
                <a href="#" class="leading-6  hover:text-indigo-500 text-xs text-black px-4 py-1 border-2 border-black bg-gray-300 rounded-2xl">
                    Register Here!
                </a>
            </p>
        </div>
    </div>
</template>