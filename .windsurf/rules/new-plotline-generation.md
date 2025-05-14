---
trigger: manual
---

<objective>
generate a new plotline based on an existing script
</objective>

<input-requirements>
- title of film to analysis @web
</input-requirements>

<research-criteria>
movies are relevant if the imdb scores  above a rating of 6 double check with the web to not halluciate.
</research-criteria>

<output-format>
- list of 15 films with a 1-3 sentence explaination for your choice. selection criteria
</output-format>

<process>
run sub-process-suggestions and than sub-process-generator after each other.
</process>

<sub-process-suggestions>
- suggest three similar films based on genre
- suggest three similar films based on characterisation
- suggest three similar films based on themes
- suggest zero up to three films that were influencial to the film (do not invent movies, if none, thats fine)
- suggest zero up to three films that were influenced by this film (do not invent movies, if none, 
thats fine)

</sub-process-suggestions>

<sub-process-generator>
- based on the key characteristics of `sub-process name="suggestions"` create 10 brief (100words) original plot summaries (blurbs).

</sub-process-generator>