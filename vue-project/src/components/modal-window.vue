<template>
    <div v-if="show" class="modal-shadow" @click.self="closeModal">
        <div class="modal">
            <div class="modal-close" @click="closeModal">&#10006;</div>
            <slot name="title">
                <h3 class="modal-title">Registration</h3>
            </slot>
            <slot name="body">
                <div class="modal-content">
                    <div class="form_sectionOne_inputs">
                        <input placeholder="Firstname"/>
                        <input placeholder="Lastname"/>
                        <input placeholder="Email address"/>
                        <button  @click="closeModal">Sign Up</button>
                    </div>
                </div>
            </slot>
        </div>
    </div>
</template>
 
<script>
    export default {
        name: "ModalWindow",
        data: function () {
            return {
                show: false
            }
        },
        methods: {
            closeModal: function () {
                this.show = false
            }
        }
    }
</script>
 
<style scoped
       lang="scss">
    .modal-shadow {
        position: absolute;
        top: 0;
        left: 0;
        min-height: 100%;
        width: 100%;
        background: rgba(0, 0, 0, 0.39);
    }

    .form_sectionOne_inputs {
        flex-direction: column;
    }

    .form_sectionOne_inputs input {
        border: 1px solid #2a4cc7;
        width: 100%;
        margin: 5px 0;
        padding: 10px;
        border-radius: 8px;
    }

    .form_sectionOne_inputs button {
        border: 1px solid #2a4cc7;
        color: white;
        cursor: pointer;
        background: linear-gradient(265.48deg, #4870FF -5.06%, #FA00FF 94.87%);
        margin: 5px 0;
        padding: 10px;
        border-radius: 8px;
    }
 
    .modal {
        background: #fff;
        border-radius: 8px;
        padding: 15px;
        width: 95%;
        max-width: 420px;
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
 
        &-close {
            border-radius: 50%;
            color: #fff;
            background: #2a4cc7;
            display: flex;
            align-items: center;
            justify-content: center;
            position: absolute;
            top: 7px;
            right: 7px;
            width: 30px;
            height: 30px;
            cursor: pointer;
        }
 
        &-title {
            color: #0971c7;
        }
 
        &-content {
            margin-bottom: 20px
        }
 
        &-footer {
            &__button {
                background-color: #0971c7;
                color: #fff;
                border: none;
                text-align: center;
                padding: 8px;
                font-size: 17px;
                font-weight: 500;
                border-radius: 8px;
                min-width: 150px;
            }
        }
    }
</style>