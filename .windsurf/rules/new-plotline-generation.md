---
trigger: manual
---

<objective>
generate a new plotline based on an existing script
</objective>

<input-requirements>
- title of film to analysis @web
</input-requirements>

<process>
- suggest three similar films based on genre
- suggest three similar films based on characterisation
- suggest three similar films based on themes
- suggest zero up to three films that were influencial to the film (do not invent movies, if none, thats fine)
- suggest zero up to three films that were influenced by this film (do not invent movies, if none, thats fine)
</process>

<research-criteria>
movies are relevant if the imdb scores  above a rating of 6 double check with the web to not halluciate.
</research-criteria>

<output-format>
- list of 9 films with a 1-3 sentence explaination for your choice
</output-format>