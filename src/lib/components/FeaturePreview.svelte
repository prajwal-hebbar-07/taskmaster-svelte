<script>
  const features = [
    {
      number: 1,
      title: "Create a ToDo List",
      strapline: "Understanding the ToDo List Creation",
      excerpt:
        "Easily create and manage your daily tasks and to-do lists. Organize your personal and professional life by adding tasks, setting reminders, and checking off completed items.",
    },
    {
      number: 2,
      title: "Task Prioritization",
      strapline: "Organize Tasks by Importance",
      excerpt:
        "Prioritize your tasks based on urgency and importance. Use labels or tags to categorize tasks and ensure you focus on high-priority items first.",
    },
    {
      number: 3,
      title: "Deadline Reminders",
      strapline: "Never Miss a Deadline Again",
      excerpt:
        "Set reminders for upcoming deadlines to ensure you never miss an important task. Receive notifications before tasks are due to help you stay on track.",
    },
    {
      number: 4,
      title: "Collaborative Lists",
      strapline: "Share and Work Together on Tasks",
      excerpt:
        "Collaborate with friends, family, or colleagues by sharing your to-do lists. Work together in real-time, assign tasks, and track progress as a team.",
    },
    {
      number: 5,
      title: "Progress Tracking",
      strapline: "Monitor Your Task Completion",
      excerpt:
        "Track your progress on tasks and to-do lists with visual indicators. See how much you've accomplished and stay motivated to complete your goals.",
    },
    {
      number: 6,
      title: "Recurring Tasks",
      strapline: "Set Up Repeating Tasks Easily",
      excerpt:
        "Automate repetitive tasks by setting them to recur at regular intervals. Save time and ensure you never forget routine tasks.",
    },
  ];

  let selectedFeatureNumber = $state(1);
  let selectedFeature = $derived(
    features.find((feature) => feature.number === selectedFeatureNumber)
  );

  function selectFeatureHandler(number) {
    selectedFeatureNumber = number;
  }
</script>

<section class="feature-preview default-margin">
  <h2 class="mb-l">Features You are Getting</h2>
  <div class="feature-container">
    <ul>
      {#each features as feature}
        <li>
          <button
            class="feature-title"
            class:selected-feature-title={selectedFeatureNumber ===
              feature.number}
            aria-controls={`feature-info-${feature.number}`}
            aria-expanded={selectedFeatureNumber === feature.number}
            onclick={() => selectFeatureHandler(feature.number)}
          >
            <h3>Feature {feature.number}: {feature.title}</h3>
          </button>
        </li>
      {/each}
    </ul>
    <div class="feature-info">
      <h3 class="feature-strapline italic mb-s">
        {selectedFeature.strapline}
      </h3>
      <p>
        {selectedFeature.excerpt}
      </p>
    </div>
  </div>
</section>

<style>
  .feature-preview {
    padding: 80px 0;
    margin-left: 12vw;
    margin-right: 20vw;
    max-width: 1150px;
  }

  .feature-container {
    display: flex;
    justify-content: space-between;
  }

  .feature-container ul {
    width: 40%;
  }

  .feature-info {
    width: 55%;
  }

  .feature-title {
    border-bottom: 1px solid grey;
    padding: 12px;
    display: block;
    width: 100%;
    text-align: left;
  }

  .selected-feature-title {
    background-color: black;
    color: white;
    border: none;
    box-shadow:
      0 4px 6px rgba(0, 0, 0, 0.1),
      0 1px 3px rgba(0, 0, 0, 0.08);
  }
</style>
