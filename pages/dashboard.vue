<template>
<div>
    <v-container>
        <v-row>

            <v-col md="2 ">

            </v-col>
            <v-col md="8">

                <v-card class="mx-auto" color="#26c6da" dark>
                    <v-card-title class="d-flex justify-end">
                        
                        <!-- <v-icon size="x-large" class="icon-spacing">mdi-eye</v-icon> -->
                        <v-icon size="x-large" class="icon-spacing">mdi-eye</v-icon>
                        <v-icon size="x-large" class="icon-spacing">mdi-magnify</v-icon>

                        <v-icon @click="openDialog" size="x-large" class="icon-spacing">mdi-pencil</v-icon>
                        <!-- Dialog Component -->
                        <v-dialog v-model="dialogVisible" max-width="500"  >
                            <v-card style="background-color: #26c6da">
                                <v-card-title>Dialog Title</v-card-title>
                                <v-card-text >
                                    <v-responsive
                                    class="mx-auto"
                                    max-width="344"
                                  >
                                    <v-text-field class="mt-5"
                                      label="Type Here..."
                                      hide-details="auto" 
                                      outlined></v-text-field>
                                  </v-responsive>
                                </v-card-text>
                                <v-card-actions>
                                    <v-btn @click="dialogVisible = false" style="background-color:rgb(0, 5, 32)">Close</v-btn>
                                </v-card-actions>
                            </v-card>
                        </v-dialog>

                    </v-card-title>

                    <hr>
                    <v-card-text class="text-h5 py-1">
                        "Cases are type invalid as"

                    </v-card-text>
                    <v-card-actions>
                        <v-list-item class="w-100">
                            <template v-slot:prepend>
                                <v-avatar color="grey darken-3" size="150">
                                    <img src="https://via.placeholder.com/150" alt="User Avatar" />
                                </v-avatar>
                            </template>
                            <v-list-item-title>Evan You</v-list-item-title>
                            <v-list-item-subtitle>Vue Creator</v-list-item-subtitle>
                            <template v-slot:append>
                                <div class="justify-self-end">
                                    <v-icon size="x-large">mdi-twitter</v-icon>
                                    <v-icon class="me-1">mdi-heart</v-icon>
                                    <span class="subheading me-2">256</span>
                                    <span class="me-1">·</span>
                                    <v-icon class="me-1">mdi-share-variant</v-icon>
                                    <span class="subheading">45</span>
                                </div>
                            </template>
                        </v-list-item>
                    </v-card-actions>
                </v-card>


                <v-card class="mx-auto mt-2" color="#26c6da" dark>
                    <v-card-title class="d-flex justify-end">
                        
                        <!-- <v-icon size="x-large" class="icon-spacing">mdi-eye</v-icon> -->
                        <v-icon size="x-large" class="icon-spacing">mdi-eye</v-icon>
                        <v-icon size="x-large" class="icon-spacing">mdi-magnify</v-icon>

                        <v-icon @click="openDialog" size="x-large" class="icon-spacing">mdi-pencil</v-icon>
                        <!-- Dialog Component -->
                        <v-dialog v-model="dialogVisible" max-width="500"  >
                            <v-card style="background-color: #26c6da">
                                <v-card-title>Dialog Title</v-card-title>
                                <v-card-text >
                                    <v-responsive
                                    class="mx-auto"
                                    max-width="344"
                                  >
                                    <v-text-field class="mt-5"
                                      label="Type Here..."
                                      hide-details="auto" 
                                      outlined></v-text-field>
                                  </v-responsive>
                                </v-card-text>
                                <v-card-actions>
                                    <v-btn @click="dialogVisible = false" style="background-color:rgb(0, 5, 32)">Close</v-btn>
                                </v-card-actions>
                            </v-card>
                        </v-dialog>

                    </v-card-title>

                    <hr>
                    <v-card-text class="text-h5 py-1">
                        "Cases are type invalid as"

                    </v-card-text>
                    <v-card-actions>
                        <v-list-item class="w-100">
                            <template v-slot:prepend>
                                <v-avatar color="grey darken-3" size="150">
                                    <img src="https://via.placeholder.com/150" alt="User Avatar" />
                                </v-avatar>
                            </template>
                            <v-list-item-title>Evan You</v-list-item-title>
                            <v-list-item-subtitle>Vue Creator</v-list-item-subtitle>
                            <template v-slot:append>
                                <div class="justify-self-end">
                                    <v-icon size="x-large">mdi-twitter</v-icon>
                                    <v-icon class="me-1">mdi-heart</v-icon>
                                    <span class="subheading me-2">256</span>
                                    <span class="me-1">·</span>
                                    <v-icon class="me-1">mdi-share-variant</v-icon>
                                    <span class="subheading">45</span>
                                </div>
                            </template>
                        </v-list-item>
                    </v-card-actions>
                </v-card>


                <v-card class="mx-auto mt-2" color="#26c6da" dark>
                    <v-card-title class="d-flex justify-end">
                        
                        <!-- <v-icon size="x-large" class="icon-spacing">mdi-eye</v-icon> -->
                        <v-icon size="x-large" class="icon-spacing">mdi-eye</v-icon>
                        <v-icon size="x-large" class="icon-spacing">mdi-magnify</v-icon>

                        <v-icon @click="openDialog" size="x-large" class="icon-spacing">mdi-pencil</v-icon>
                        <!-- Dialog Component -->
                        <v-dialog v-model="dialogVisible" max-width="500"  >
                            <v-card style="background-color: #26c6da">
                                <v-card-title>Dialog Title</v-card-title>
                                <v-card-text >
                                    <v-responsive
                                    class="mx-auto"
                                    max-width="344"
                                  >
                                    <v-text-field class="mt-5"
                                      label="Type Here..."
                                      hide-details="auto" 
                                      outlined></v-text-field>
                                  </v-responsive>
                                </v-card-text>
                                <v-card-actions>
                                    <v-btn @click="dialogVisible = false" style="background-color:rgb(0, 5, 32)">Close</v-btn>
                                </v-card-actions>
                            </v-card>
                        </v-dialog>

                    </v-card-title>

                    <hr>
                    <v-card-text class="text-h5 py-1">
                        "Cases are type invalid as"

                    </v-card-text>
                    <v-card-actions>
                        <v-list-item class="w-100">
                            <template v-slot:prepend>
                                <v-avatar color="grey darken-3" size="150">
                                    <img src="https://via.placeholder.com/150" alt="User Avatar" />
                                </v-avatar>
                            </template>
                            <v-list-item-title>Evan You</v-list-item-title>
                            <v-list-item-subtitle>Vue Creator</v-list-item-subtitle>
                            <template v-slot:append>
                                <div class="justify-self-end">
                                    <v-icon size="x-large">mdi-twitter</v-icon>
                                    <v-icon class="me-1">mdi-heart</v-icon>
                                    <span class="subheading me-2">256</span>
                                    <span class="me-1">·</span>
                                    <v-icon class="me-1">mdi-share-variant</v-icon>
                                    <span class="subheading">45</span>
                                </div>
                            </template>
                        </v-list-item>
                    </v-card-actions>
                </v-card>


                <v-card class="mx-auto mt-2" color="#26c6da" dark>
                    <v-card-title class="d-flex justify-end">
                        
                        <!-- <v-icon size="x-large" class="icon-spacing">mdi-eye</v-icon> -->
                        <v-icon size="x-large" class="icon-spacing">mdi-eye</v-icon>
                        <v-icon size="x-large" class="icon-spacing">mdi-magnify</v-icon>

                        <v-icon @click="openDialog" size="x-large" class="icon-spacing">mdi-pencil</v-icon>
                        <!-- Dialog Component -->
                        <v-dialog v-model="dialogVisible" max-width="500"  >
                            <v-card style="background-color: #26c6da">
                                <v-card-title>Dialog Title</v-card-title>
                                <v-card-text >
                                    <v-responsive
                                    class="mx-auto"
                                    max-width="344"
                                  >
                                    <v-text-field class="mt-5"
                                      label="Type Here..."
                                      hide-details="auto" 
                                      outlined></v-text-field>
                                  </v-responsive>
                                </v-card-text>
                                <v-card-actions>
                                    <v-btn @click="dialogVisible = false" style="background-color:rgb(0, 5, 32)">Close</v-btn>
                                </v-card-actions>
                            </v-card>
                        </v-dialog>

                    </v-card-title>

                    <hr>
                    <v-card-text class="text-h5 py-1">
                        "Cases are type invalid as"

                    </v-card-text>
                    <v-card-actions>
                        <v-list-item class="w-100">
                            <template v-slot:prepend>
                                <v-avatar color="grey darken-3" size="150">
                                    <img src="https://via.placeholder.com/150" alt="User Avatar" />
                                </v-avatar>
                            </template>
                            <v-list-item-title>Evan You</v-list-item-title>
                            <v-list-item-subtitle>Vue Creator</v-list-item-subtitle>
                            <template v-slot:append>
                                <div class="justify-self-end">
                                    <v-icon size="x-large">mdi-twitter</v-icon>
                                    <v-icon class="me-1">mdi-heart</v-icon>
                                    <span class="subheading me-2">256</span>
                                    <span class="me-1">·</span>
                                    <v-icon class="me-1">mdi-share-variant</v-icon>
                                    <span class="subheading">45</span>
                                </div>
                            </template>
                        </v-list-item>
                    </v-card-actions>
                </v-card>





               

                <v-card class="mx-auto mt-2" color="#26c6da" theme="dark" prepend-icon="mdi-twitter" title="Twitter">
                    <template v-slot:prepend>
                        <v-icon size="x-large"></v-icon>
                    </template>

                    <v-card-text class="text-h5 py-2">
                        " cases are type invalid as "
                    </v-card-text>

                    <v-card-actions>
                        <v-list-item class="w-100">
                            <template v-slot:prepend>
                                <v-avatar color="grey-darken-3" image="https://via.placeholder.com/150"></v-avatar>
                            </template>

                            <v-list-item-title>Evan You</v-list-item-title>

                            <v-list-item-subtitle>Vue Creator</v-list-item-subtitle>

                            <template v-slot:append>
                                <div class="justify-self-end">
                                    <v-icon class="me-1" icon="mdi-heart"></v-icon>
                                    <span class="subheading me-2">256</span>
                                    <span class="me-1">·</span>
                                    <v-icon class="me-1" icon="mdi-share-variant"></v-icon>
                                    <span class="subheading">45</span>
                                </div>
                            </template>
                        </v-list-item>
                    </v-card-actions>
                </v-card>

            </v-col>

            <v-col md="2">

            </v-col>

        </v-row>
    </v-container>
    <!-- <h1>dashboard</h1> -->
</div>
</template>

<script>
 export default {
  data() {
    return {
      dialogVisible: false,
    };
  },
  methods: {
    openDialog() {
      this.dialogVisible = true;
    },
  },
};
  </script>

<style>
.icon-spacing {
    margin-right: 8px;
    /* Adjust this value for your desired spacing */
}



</style>
